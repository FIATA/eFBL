# Standardized Identifier Schema

```txt
https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json
```

Identifier which identification scheme is maintained by an external agency

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                           |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [standardized-identifier.schema.json](../tooling/out/definitions/classes/standardized-identifier.schema.json "open original schema") |

## Standardized Identifier Type

`object` ([Standardized Identifier](standardized-identifier.md))

# Standardized Identifier Properties

| Property                                                  | Type     | Required | Nullable       | Defined by                                                                                                                                                  |
| :-------------------------------------------------------- | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [value](#value)                                           | `string` | Required | cannot be null | [Standardized Identifier](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/value")                      |
| [identificationScheme](#identificationscheme)             | `string` | Optional | cannot be null | [Standardized Identifier](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/identificationScheme")       |
| [identificationSchemeAgency](#identificationschemeagency) | `string` | Optional | cannot be null | [Standardized Identifier](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/identificationSchemeAgency") |

## value

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`value`

*   is required

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Standardized Identifier](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/value")

### value Type

`string` ([Identifier](identifier.md))

## identificationScheme

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`identificationScheme`

*   is optional

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Standardized Identifier](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/identificationScheme")

### identificationScheme Type

`string` ([Identifier](identifier.md))

## identificationSchemeAgency

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`identificationSchemeAgency`

*   is optional

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Standardized Identifier](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/identificationSchemeAgency")

### identificationSchemeAgency Type

`string` ([Identifier](identifier.md))
