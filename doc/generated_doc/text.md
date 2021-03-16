# Text Schema

```txt
https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json
```

The text with optional localization.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                     |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :--------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [text.schema.json](../tooling/out/definitions/classes/text.schema.json "open original schema") |

## Text Type

`object` ([Text](text.md))

# Text Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                       |
| :-------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| [value](#value)       | `string` | Required | cannot be null | [Text](text-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/properties/value") |
| [language](#language) | `string` | Optional | cannot be null | [Text](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/language")           |

## value

A character string (i.e. a finite set of characters) generally in the form of words of a language.

`value`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Text](text-properties-value.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/properties/value")

### value Type

`string`

## language

A character string to identify and distinguish uniquely, one instance of an object in an identification scheme from all other objects within the same scheme.

`language`

*   is optional

*   Type: `string` ([Identifier](identifier.md))

*   cannot be null

*   defined in: [Text](identifier.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/language")

### language Type

`string` ([Identifier](identifier.md))
