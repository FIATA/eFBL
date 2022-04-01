# Paperless FIATA Bill of Lading generating and tracking services

## Pre-Requisites

### Agreement with FIATA

Before being able to issue paperless FIATA Bill of Lading using the provided APIs, any organization (software provider, 
freight forwarding company, ...) you need to register with FIATA and sign a standard agreement. Once the agreement signed,
you will receive all the details for connecting to the service.

In order to subscribe to the service, please contact directly [FIATA Head-Quarters](https://www.fiata.org). 

### Software Provider ID

After signing the agreement with FIATA, you will be assigned a Software Provider identifier that you will pass as parameter 
of the request to the service.

### Freight Forwarder ID

Any Freight Forwarder company buying a package of paperless FIATA Bills of Lading will be assigned a unique identifier. 
This unique identifier needs to be inserted in the Bill of Lading body of the request in the CTO object.

### Paperless package order

In order to issue paperless FIATA Bills of Lading, Freight Forwarders companies need to buy packages. You can find
more information on [FIATA website](https://www.fiata.org)

## Operations

You can find a sample collection of all possible calls in the Postman collection in the examples folder of this repository.
Please note that the Postman collection does not contain any server address, identifiers or secrets. The example request 
use variables defined at the level of the collection that you can define with the information you receive by FIATA upon
registration

### Authentication

#### Request
The authentication request is defined in the following sections

##### Call

| Element      | Value                                                                             |
|--------------|-----------------------------------------------------------------------------------|
| Method       | POST                                                                              |
| URL Pattern  | ``` {{authentication_server}}/auth/realms/fiata/protocol/openid-connect/token ``` |

##### Headers

| Header       | Value                               |
|--------------|-------------------------------------|
| Content-Type | `application/x-www-form-urlencoded` |


##### Request Body

| Key             | Description                                                                             |
|-----------------|-----------------------------------------------------------------------------------------|
| `username`      | The service credential username. Provided by FIATA during the on-boarding process       |
| `password`      | The service credential password. Provided by FIATA during the on-boarding process       |
| `client_id`     | The client identifier for the service. Provided by FIATA during the on-boarding process |
| `client_secret` | The client secret. Provided by FIATA during the on-boarding process                     |
| `grant_type`    | Value must be ```password```                                                            |

#### Response

A successful call to the authentication service will result in a JSON response with the needed tokens to be used in the
subsequent calls.

The `access_token` value of the body is to be used for subsequent calls to the service. See below 

The following code shows a typical answer of the authentication call:

##### Headers

| Header       | Value              |
|--------------|--------------------|
| Content-Type | `application/json` |

##### Response Body

```json
{
    "access_token": "eyJhbGciOiJS...",
    "expires_in": 300,
    "refresh_expires_in": 1800,
    "refresh_token": "eyJhbGciOiJIUz...",
    "token_type": "bearer",
    "not-before-policy": 0,
    "session_state": "405865c5-eb48-4227-afde-8309256427dc",
    "scope": "profile email"
}
```

### Document Issuance

The service allows you to produce versions of the FIATA Bill of Lading. There are three ways of producing documents:

| Name      | Activation                                                | Description                                                                                                                                                                         |
|-----------|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Preview   | `mode=preview` request parameter                          | This produces draft a version of the document based on the model. **Draft versions are not registered and cannot be verified**                                                      |
| Issuance  | Standard request                                          | This produces and registers a document. The document can then be verified as long as it is not deactivated                                                                          |
| Amendment | Defined `exchanged_document/id` value in the request body | This allows to produce a new version of an existing registered document. **Previous versions of an amended document will not be verifiable anymore and thus considered as invalid** |


#### Request specification

##### Call

| Element      | Value                                                               |
|--------------|---------------------------------------------------------------------|
| Method       | POST                                                                |
| URL Pattern  | ``` {{api_server}}/api/trakk/v0/integrations/fiata/fbl-json ```     |

##### Meaningful Headers

| Header        | Value                     | Note                                                    |
|---------------|---------------------------|---------------------------------------------------------|
| Content-Type  | `application/json`        |                                                         |
| Authorization | `Bearer {{access_token}}` | Please insert the token retrieved in the Authentication |
| X-Alias-ID    | `fiata`                   | Constant to be included                                 |


##### Query Paramaters

| Query psarameter name | Type     | Value                                                                                                            |
|-----------------------|----------|------------------------------------------------------------------------------------------------------------------|
| `softwareProviderId`  | Required | The software provider id delivered during the software provider onboarding process                               |
| `mode`                | Optional | In order to generate preview documents, use the value `preview` for this parameter. All other values are ignored |


##### Request Body

The body contains a well-formed JSON document respecting the [standard eFBL JSON schema](./schema_doc.html) 

The JSON document *MUST* contain the identifier of the Freight Forwarder ID in the [`supply_chain_consigment/cto/id` property](./schema_doc.html#supply_chain_consignment_cto). 

When generating an amendment of an existing document the provided JSON document must contain the id of an existing document in the [`exchanged_document/id` property](./schema_doc.html#exchanged_document_id).
The unique identifier of the document is provided in the returned filename.

#### Successful Response

A successful response contains a PDF document of the FIATA Bill of Lading. Depending on the conditons, the document can be either:

1. A preview document
2. A new registered document 
3. A new amended version of an existing document

##### Meaningful Headers

| Header              | Value                                                 | Note                                                                                                                                                                                                                                                   |
|---------------------|-------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Content-Type        | `application/pdf`                                     |                                                                                                                                                                                                                                                        |
| Transfer-Encoding   | `chunked`                                             |                                                                                                                                                                                                                                                        |
| Content-Disposition | `attachment; filename={{eFBL unique identifier}}.pdf` | The attachment filename contains the unique identifier of the generated document. This identifier can be subsequently used for generating amendments. Please note that identifiers of preview documents are volatile and cannot be used for amendments |

##### Response Body

The preview PDF document of the FIATA Bill of Lading. **Preview documents are not registered and cannot be verified**

#### Error Response - Invalid body

If the body contains an invalid but well formatted JSON document, the service will return a document containing the 
validation errors.

##### Status

`400 Bad Request`

##### Meaningful Headers

| Header        | Value                            | Note                                                    |
|---------------|----------------------------------|---------------------------------------------------------|
| Content-Type  | `application/json;charset=utf-8` |                                                         |

##### Response Body

This is a simplified error example because of missing required `issueDateTime` field in the `exchanged_document` part

```json
{
    "errorCode": "EDAT02",
    "message": "Trakk document is not registered",
    "origin": "api-trakk",
    "fields": {
      "errors": [
        {
          "keyword": "required",
          "dataPath": ".exchanged_document",
          "schemaPath": "#/required",
          "params": {
            "missingProperty": "issueDateTime"
          },
          "message": "should have required property 'issueDateTime'",
          "schema": {
            [...]
          }
        }
      ]
    }
}
``` 

#### Error Response - Missing or wrong Software ID

If the request is sent with an invalid software identifier in the `softwareProviderId` query parameter, the call will 
result in an error response

##### Status

`401 Unauthorized`


#### Error Response - Amendment of a unregistered document

If the request is sent with an invalid document identifier in the `exchanged_document/id` property of the request body, 
the call will result in an error response. Please note that a document identifier of a preview document is considered as invalid.

##### Status

`400 Bad Request`


