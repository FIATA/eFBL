# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty
```



| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## tradeParty Type

`object` ([Details](supply-chain-consignment-defs-tradeparty.md))

# tradeParty Properties

| Property                                          | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                               |
| :------------------------------------------------ | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                                         | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-id.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/id")                                         |
| [name](#name)                                     | `object` | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/tradeParty/properties/name")                                                                                                      |
| [languageCode](#languagecode)                     | `object` | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/tradeParty/properties/languageCode")                                                                                              |
| [definedContactDetails](#definedcontactdetails)   | `object` | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/definedContactDetails")                                  |
| [postalAddress](#postaladdress)                   | `object` | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/postalAddress")                                          |
| [taxRegistration](#taxregistration)               | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-taxregistration.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/taxRegistration")               |
| [governmentRegistration](#governmentregistration) | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-governmentregistration.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/governmentRegistration") |

## id

A unique identifier of this trade party.

`id`

*   is optional

*   Type: `object[]` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-id.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/id")

### id Type

`object[]` ([Standardized Identifier](standardized-identifier.md))

## name

The text with optional localization.

`name`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/tradeParty/properties/name")

### name Type

`object` ([Text](text.md))

## languageCode

A code.

`languageCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/tradeParty/properties/languageCode")

### languageCode Type

`object` ([Code](code.md))

## definedContactDetails

A trade contact defined for this trade party.

`definedContactDetails`

*   is optional

*   Type: `object` ([Details](supply-chain-consignment-defs-tradecontact.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/definedContactDetails")

### definedContactDetails Type

`object` ([Details](supply-chain-consignment-defs-tradecontact.md))

## postalAddress

The postal address for this trade party.

`postalAddress`

*   is optional

*   Type: `object` ([Details](supply-chain-consignment-defs-tradeaddress.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/postalAddress")

### postalAddress Type

`object` ([Details](supply-chain-consignment-defs-tradeaddress.md))

## taxRegistration

A tax registration specified for this trade party.

`taxRegistration`

*   is optional

*   Type: `object[]` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-taxregistration.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/taxRegistration")

### taxRegistration Type

`object[]` ([Standardized Identifier](standardized-identifier.md))

## governmentRegistration

A governmental registration specified for this trade party.

`governmentRegistration`

*   is optional

*   Type: `object[]` ([Details](supply-chain-consignment-defs-governmentregistration.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-governmentregistration.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/governmentRegistration")

### governmentRegistration Type

`object[]` ([Details](supply-chain-consignment-defs-governmentregistration.md))
