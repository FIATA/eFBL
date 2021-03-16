# Measure Schema

```txt
https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json
```

A measure with its unit.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                           |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :--------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [measure.schema.json](../tooling/out/definitions/classes/measure.schema.json "open original schema") |

## Measure Type

`object` ([Measure](measure.md))

# Measure Properties

| Property        | Type     | Required | Nullable       | Defined by                                                                                                                                |
| :-------------- | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| [value](#value) | `number` | Required | cannot be null | [Measure](measure-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/properties/value") |
| [unit](#unit)   | `string` | Optional | cannot be null | [Measure](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/unit")                     |

## value



`value`

*   is required

*   Type: `number`

*   cannot be null

*   defined in: [Measure](measure-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/properties/value")

### value Type

`number`

## unit

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`unit`

*   is optional

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Measure](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/unit")

### unit Type

`string` ([Identifier](identifier.md))
