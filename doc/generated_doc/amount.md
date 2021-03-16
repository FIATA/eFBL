# Amount Schema

```txt
https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json
```

A number of monetary units specified in a currency where the unit of the currency is explicit or implied.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [amount.schema.json](../tooling/out/definitions/classes/amount.schema.json "open original schema") |

## Amount Type

`object` ([Amount](amount.md))

# Amount Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                             |
| :-------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------- |
| [value](#value)       | `number` | Required | cannot be null | [Amount](amount-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/properties/value") |
| [currency](#currency) | `string` | Optional | cannot be null | [Amount](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/currency")               |

## value



`value`

*   is required

*   Type: `number`

*   cannot be null

*   defined in: [Amount](amount-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/properties/value")

### value Type

`number`

## currency

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`currency`

*   is optional

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Amount](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/currency")

### currency Type

`string` ([Identifier](identifier.md))
