# Document Authentication Schema

```txt
https://fiata.com/digital/schemas/json/definitions/classes/document-authentication.schema.json
```

The first or primary signature that authenticates a document.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                           |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [document-authentication.schema.json](../tooling/out/definitions/classes/document-authentication.schema.json "open original schema") |

## Document Authentication Type

`object` ([Document Authentication](document-authentication.md))

# Document Authentication Properties

| Property                          | Type     | Required | Nullable       | Defined by                                                                                                                                            |
| :-------------------------------- | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------- |
| [actualDateTime](#actualdatetime) | `object` | Required | cannot be null | [Document Authentication](date-time.md "https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json#/properties/actualDateTime") |
| [identifier](#identifier)         | `string` | Optional | cannot be null | [Document Authentication](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/identifier")           |
| [statement](#statement)           | `object` | Optional | cannot be null | [Document Authentication](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/properties/statement")                |

## actualDateTime

The date, time, date time or other date time value.

`actualDateTime`

*   is required

*   Type: `object` ([Date Time](date-time.md))

*   cannot be null

*   defined in: [Document Authentication](date-time.md "https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json#/properties/actualDateTime")

### actualDateTime Type

`object` ([Date Time](date-time.md))

## identifier

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`identifier`

*   is optional

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Document Authentication](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/identifier")

### identifier Type

`string` ([Identifier](identifier.md))

## statement

The text with optional localization.

`statement`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Document Authentication](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/properties/statement")

### statement Type

`object` ([Text](text.md))
