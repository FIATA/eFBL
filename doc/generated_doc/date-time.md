# Date Time Schema

```txt
https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json
```

The date, time, date time or other date time value.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                               |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [date-time.schema.json](../tooling/out/definitions/classes/date-time.schema.json "open original schema") |

## Date Time Type

`object` ([Date Time](date-time.md))

# Date Time Properties

| Property          | Type     | Required | Nullable       | Defined by                                                                                                                                        |
| :---------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------ |
| [value](#value)   | `string` | Required | cannot be null | [Date Time](date-time-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json#/properties/value")   |
| [format](#format) | `string` | Optional | cannot be null | [Date Time](date-time-properties-format.md "https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json#/properties/format") |

## value

The particular point in the progression of time.

`value`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Date Time](date-time-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json#/properties/value")

### value Type

`string`

## format

The format of the date/time content.

`format`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Date Time](date-time-properties-format.md "https://fiata.com/digital/schemas/json/definitions/classes/date-time.schema.json#/properties/format")

### format Type

`string`
