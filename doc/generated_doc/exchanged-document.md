# Exchanged Document Schema

```txt
https://fiata.com/digital/schemas/json/definitions/exchanged-document.schema.json
```

Exchanged Document

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                         |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [exchanged-document.schema.json](../tooling/out/definitions/exchanged-document.schema.json "open original schema") |

## Exchanged Document Type

`object` ([Exchanged Document](exchanged-document.md))

# Exchanged Document Properties

| Property                                                      | Type          | Required | Nullable       | Defined by                                                                                                                                                                                 |
| :------------------------------------------------------------ | :------------ | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                                                     | `string`      | Optional | cannot be null | [Exchanged Document](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/id")                                                             |
| [issueDateTime](#issuedatetime)                               | `object`      | Optional | cannot be null | [Exchanged Document](date-time.md "https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json#/properties/issueDateTime")                                            |
| [originalIssuedQuantity](#originalissuedquantity)             | `number`      | Required | cannot be null | [Exchanged Document](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/originalIssuedQuantity")                                           |
| [copyIssuedQuantity](#copyissuedquantity)                     | `number`      | Optional | cannot be null | [Exchanged Document](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/copyIssuedQuantity")                                               |
| [issueLocation](#issuelocation)                               | Not specified | Required | cannot be null | [Exchanged Document](exchanged-document-properties-issuelocation.md "https://fiata.com/digital/schemas/json/definitions/exchanged-document.schema.json#/properties/issueLocation")         |
| [firstSignatoryAuthentication](#firstsignatoryauthentication) | `object`      | Optional | cannot be null | [Exchanged Document](document-authentication.md "https://fiata.com/digital/schemas/json/definitions/classes/document-authentication.schema.json#/properties/firstSignatoryAuthentication") |

## id

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`id`

*   is optional

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Exchanged Document](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/id")

### id Type

`string` ([Identifier](identifier.md))

## issueDateTime

The date, time, date time or other date time value.

`issueDateTime`

*   is optional

*   Type: `object` ([Date Time](date-time.md))

*   cannot be null

*   defined in: [Exchanged Document](date-time.md "https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json#/properties/issueDateTime")

### issueDateTime Type

`object` ([Date Time](date-time.md))

## originalIssuedQuantity

A counted number of non-monetary units possibly including fractions.

`originalIssuedQuantity`

*   is required

*   Type: `number` ([Identifier](quantity.md))

*   cannot be null

*   defined in: [Exchanged Document](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/originalIssuedQuantity")

### originalIssuedQuantity Type

`number` ([Identifier](quantity.md))

## copyIssuedQuantity

A counted number of non-monetary units possibly including fractions.

`copyIssuedQuantity`

*   is optional

*   Type: `number` ([Identifier](quantity.md))

*   cannot be null

*   defined in: [Exchanged Document](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/copyIssuedQuantity")

### copyIssuedQuantity Type

`number` ([Identifier](quantity.md))

## issueLocation

The location where this exchanged document has been issued.

`issueLocation`

*   is required

*   Type: unknown

*   cannot be null

*   defined in: [Exchanged Document](exchanged-document-properties-issuelocation.md "https://fiata.com/digital/schemas/json/definitions/exchanged-document.schema.json#/properties/issueLocation")

### issueLocation Type

unknown

## firstSignatoryAuthentication

The first or primary signature that authenticates a document.

`firstSignatoryAuthentication`

*   is optional

*   Type: `object` ([Document Authentication](document-authentication.md))

*   cannot be null

*   defined in: [Exchanged Document](document-authentication.md "https://fiata.com/digital/schemas/json/definitions/classes/document-authentication.schema.json#/properties/firstSignatoryAuthentication")

### firstSignatoryAuthentication Type

`object` ([Document Authentication](document-authentication.md))
