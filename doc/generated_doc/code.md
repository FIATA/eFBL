# Code Schema

```txt
https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json
```

A code.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :--------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [code.schema.json](../tooling/out/definitions/classes/code.schema.json "open original schema") |

## Code Type

`object` ([Code](code.md))

# Code Properties

| Property          | Type     | Required | Nullable       | Defined by                                                                                                                       |
| :---------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| [value](#value)   | `string` | Required | cannot be null | [Code](code-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/properties/value") |
| [agency](#agency) | `string` | Optional | cannot be null | [Code](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/agency")             |

## value



`value`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Code](code-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/properties/value")

### value Type

`string`

## agency

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`agency`

*   is optional

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Code](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/agency")

### agency Type

`string` ([Identifier](identifier.md))
