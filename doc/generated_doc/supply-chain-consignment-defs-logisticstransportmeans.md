# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsTransportMeans
```

The means of transport used for this logistics transport movement.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## logisticsTransportMeans Type

`object` ([Details](supply-chain-consignment-defs-logisticstransportmeans.md))

# logisticsTransportMeans Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                           |
| :-------------------- | :------- | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [typeCode](#typecode) | `object` | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/logisticsTransportMeans/properties/typeCode")                                 |
| [typeText](#typetext) | `object` | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/logisticsTransportMeans/properties/typeText")                                 |
| [id](#id)             | `object` | Optional | cannot be null | [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/logisticsTransportMeans/properties/id") |
| [name](#name)         | `object` | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/logisticsTransportMeans/properties/name")                                     |

## typeCode

A code.

`typeCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/logisticsTransportMeans/properties/typeCode")

### typeCode Type

`object` ([Code](code.md))

## typeText

The text with optional localization.

`typeText`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/logisticsTransportMeans/properties/typeText")

### typeText Type

`object` ([Text](text.md))

## id

Identifier which identification scheme is maintained by an external agency

`id`

*   is optional

*   Type: `object` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/logisticsTransportMeans/properties/id")

### id Type

`object` ([Standardized Identifier](standardized-identifier.md))

## name

The text with optional localization.

`name`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/logisticsTransportMeans/properties/name")

### name Type

`object` ([Text](text.md))
