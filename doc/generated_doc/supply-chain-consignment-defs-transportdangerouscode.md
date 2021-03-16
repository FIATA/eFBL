# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/transportDangerousCode
```

Dangerous goods transport details applicable to this supply chain consignment item.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## transportDangerousCode Type

`object` ([Details](supply-chain-consignment-defs-transportdangerouscode.md))

# transportDangerousCode Properties

| Property                                          | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                              |
| :------------------------------------------------ | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [undgId](#undgid)                                 | `object` | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/transportDangerousCode/properties/undgId")                                                       |
| [hazardClassificationId](#hazardclassificationid) | `object` | Optional | cannot be null | [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/transportDangerousCode/properties/hazardClassificationId") |

## undgId

A code.

`undgId`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/transportDangerousCode/properties/undgId")

### undgId Type

`object` ([Code](code.md))

## hazardClassificationId

Identifier which identification scheme is maintained by an external agency

`hazardClassificationId`

*   is optional

*   Type: `object` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/transportDangerousCode/properties/hazardClassificationId")

### hazardClassificationId Type

`object` ([Standardized Identifier](standardized-identifier.md))
