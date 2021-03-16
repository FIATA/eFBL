# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/transportCargo
```

Transport cargo details of this supply chain consignment item sufficient to identify its nature for customs, statistical or transport purposes.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## transportCargo Type

`object` ([Details](supply-chain-consignment-defs-transportcargo.md))

# transportCargo Properties

| Property                                  | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                               |
| :---------------------------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [typeCode](#typecode)                     | `object` | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/transportCargo/properties/typeCode")                                                                                              |
| [identificationText](#identificationtext) | `array`  | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-transportcargo-properties-identificationtext.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/transportCargo/properties/identificationText") |

## typeCode

A code.

`typeCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/transportCargo/properties/typeCode")

### typeCode Type

`object` ([Code](code.md))

## identificationText

Identification, expressed as text, of this transport cargo that is sufficient to identify it for customs, statistical or transport purposes.

`identificationText`

*   is required

*   Type: `object[]` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-transportcargo-properties-identificationtext.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/transportCargo/properties/identificationText")

### identificationText Type

`object[]` ([Text](text.md))

### identificationText Constraints

**minimum number of items**: the minimum number of items for this array is: `1`
