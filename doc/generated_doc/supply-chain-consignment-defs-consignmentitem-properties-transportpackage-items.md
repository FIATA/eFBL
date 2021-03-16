# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportPackage/items
```

A transport package for this supply chain consignment item.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## items Type

`object` ([Details](supply-chain-consignment-defs-consignmentitem-properties-transportpackage-items.md))

# items Properties

| Property                        | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                         |
| :------------------------------ | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [itemQuantity](#itemquantity)   | `number` | Optional | cannot be null | [Supply Chain Consignment](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/$defs/logisticsPackage/properties/itemQuantity")                                                                                |
| [typeCode](#typecode)           | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-typecode.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/typeCode")           |
| [typeText](#typetext)           | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-typetext.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/typeText")           |
| [shippingMarks](#shippingmarks) | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-shippingmarks.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/shippingMarks") |

## itemQuantity

A counted number of non-monetary units possibly including fractions.

`itemQuantity`

*   is optional

*   Type: `number` ([Identifier](quantity.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/$defs/logisticsPackage/properties/itemQuantity")

### itemQuantity Type

`number` ([Identifier](quantity.md))

## typeCode

A code specifying the type of logistics package.

`typeCode`

*   is optional

*   Type: `object[]` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-typecode.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/typeCode")

### typeCode Type

`object[]` ([Code](code.md))

## typeText

A type, expressed as text, of this logistics package.

`typeText`

*   is optional

*   Type: `object[]` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-typetext.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/typeText")

### typeText Type

`object[]` ([Text](text.md))

## shippingMarks

Physical shipping marks and barcode information for this logistics package.

`shippingMarks`

*   is optional

*   Type: `object[]` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-shippingmarks.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/shippingMarks")

### shippingMarks Type

`object[]` ([Text](text.md))
