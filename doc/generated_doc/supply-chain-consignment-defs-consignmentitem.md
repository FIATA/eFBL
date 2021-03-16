# Untitled undefined type in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem
```

A consignment item included in this supply chain consignment.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## consignmentItem Type

unknown

# consignmentItem Properties

| Property                                                          | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                                                           |
| :---------------------------------------------------------------- | :------------ | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [goodsTypeCode](#goodstypecode)                                   | `object`      | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/consignmentItem/properties/goodsTypeCode")                                                                                                    |
| [declaredValueForCarriageAmount](#declaredvalueforcarriageamount) | `object`      | Optional | cannot be null | [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/$defs/consignmentItem/properties/declaredValueForCarriageAmount")                                                                               |
| [insuranceValueAmount](#insurancevalueamount)                     | `object`      | Optional | cannot be null | [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/$defs/consignmentItem/properties/insuranceValueAmount")                                                                                         |
| [grossWeight](#grossweight)                                       | `object`      | Optional | cannot be null | [Supply Chain Consignment](measure.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/$defs/consignmentItem/properties/grossWeight")                                                                                                |
| [grossVolume](#grossvolume)                                       | `object`      | Optional | cannot be null | [Supply Chain Consignment](measure.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/$defs/consignmentItem/properties/grossVolume")                                                                                                |
| [cargoNatureIdentification](#cargonatureidentification)           | `object`      | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-transportcargo.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/cargoNatureIdentification")                                   |
| [transportDangerousGoods](#transportdangerousgoods)               | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-consignmentitem-properties-transportdangerousgoods.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportDangerousGoods") |
| [transportPackage](#transportpackage)                             | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-consignmentitem-properties-transportpackage.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportPackage")               |

## goodsTypeCode

A code.

`goodsTypeCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/consignmentItem/properties/goodsTypeCode")

### goodsTypeCode Type

`object` ([Code](code.md))

## declaredValueForCarriageAmount

A number of monetary units specified in a currency where the unit of the currency is explicit or implied.

`declaredValueForCarriageAmount`

*   is optional

*   Type: `object` ([Amount](amount.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/$defs/consignmentItem/properties/declaredValueForCarriageAmount")

### declaredValueForCarriageAmount Type

`object` ([Amount](amount.md))

## insuranceValueAmount

A number of monetary units specified in a currency where the unit of the currency is explicit or implied.

`insuranceValueAmount`

*   is optional

*   Type: `object` ([Amount](amount.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/$defs/consignmentItem/properties/insuranceValueAmount")

### insuranceValueAmount Type

`object` ([Amount](amount.md))

## grossWeight

A measure with its unit.

`grossWeight`

*   is optional

*   Type: `object` ([Measure](measure.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](measure.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/$defs/consignmentItem/properties/grossWeight")

### grossWeight Type

`object` ([Measure](measure.md))

## grossVolume

A measure with its unit.

`grossVolume`

*   is optional

*   Type: `object` ([Measure](measure.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](measure.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/$defs/consignmentItem/properties/grossVolume")

### grossVolume Type

`object` ([Measure](measure.md))

## cargoNatureIdentification

Transport cargo details of this supply chain consignment item sufficient to identify its nature for customs, statistical or transport purposes.

`cargoNatureIdentification`

*   is required

*   Type: `object` ([Details](supply-chain-consignment-defs-transportcargo.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-transportcargo.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/cargoNatureIdentification")

### cargoNatureIdentification Type

`object` ([Details](supply-chain-consignment-defs-transportcargo.md))

## transportDangerousGoods

Dangerous goods transport details applicable to this supply chain consignment item.

`transportDangerousGoods`

*   is optional

*   Type: `object[]` ([Details](supply-chain-consignment-defs-transportdangerouscode.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-consignmentitem-properties-transportdangerousgoods.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportDangerousGoods")

### transportDangerousGoods Type

`object[]` ([Details](supply-chain-consignment-defs-transportdangerouscode.md))

## transportPackage

A transport package for this supply chain consignment item.

`transportPackage`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-consignmentitem-properties-transportpackage.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportPackage")

### transportPackage Type

unknown
