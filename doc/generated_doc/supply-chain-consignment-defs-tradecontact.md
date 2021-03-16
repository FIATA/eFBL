# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeContact
```



| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## tradeContact Type

`object` ([Details](supply-chain-consignment-defs-tradecontact.md))

# tradeContact Properties

| Property                            | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                                     |
| :---------------------------------- | :------------ | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [personName](#personname)           | `object`      | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/tradeContact/properties/personName")                                                                                    |
| [telephone](#telephone)             | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-complete-number.md "https://fiata.com/digital/schemas/json/definitions/classes/complete-number.schema.json#/$defs/tradeContact/properties/telephone")         |
| [mobileTelephone](#mobiletelephone) | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-complete-number-1.md "https://fiata.com/digital/schemas/json/definitions/classes/complete-number.schema.json#/$defs/tradeContact/properties/mobileTelephone") |
| [emailAddress](#emailaddress)       | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-uri.md "https://fiata.com/digital/schemas/json/definitions/classes/uri.schema.json#/$defs/tradeContact/properties/emailAddress")                              |
| [note](#note)                       | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-note.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeContact/properties/note")                       |

## personName

The text with optional localization.

`personName`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/tradeContact/properties/personName")

### personName Type

`object` ([Text](text.md))

## telephone

Telephone communication information for this trade contact.

`telephone`

*   is optional

*   Type: unknown ([Complete Number](supply-chain-consignment-defs-tradecontact-properties-complete-number.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-complete-number.md "https://fiata.com/digital/schemas/json/definitions/classes/complete-number.schema.json#/$defs/tradeContact/properties/telephone")

### telephone Type

unknown ([Complete Number](supply-chain-consignment-defs-tradecontact-properties-complete-number.md))

## mobileTelephone

The mobile telephone communication information for this trade contact.

`mobileTelephone`

*   is optional

*   Type: unknown ([Complete Number](supply-chain-consignment-defs-tradecontact-properties-complete-number-1.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-complete-number-1.md "https://fiata.com/digital/schemas/json/definitions/classes/complete-number.schema.json#/$defs/tradeContact/properties/mobileTelephone")

### mobileTelephone Type

unknown ([Complete Number](supply-chain-consignment-defs-tradecontact-properties-complete-number-1.md))

## emailAddress

The email URI communication information for this trade contact.

`emailAddress`

*   is optional

*   Type: unknown ([URI](supply-chain-consignment-defs-tradecontact-properties-uri.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-uri.md "https://fiata.com/digital/schemas/json/definitions/classes/uri.schema.json#/$defs/tradeContact/properties/emailAddress")

### emailAddress Type

unknown ([URI](supply-chain-consignment-defs-tradecontact-properties-uri.md))

## note

A note specified for this trade contact.

`note`

*   is optional

*   Type: `object[]` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-note.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeContact/properties/note")

### note Type

`object[]` ([Text](text.md))
