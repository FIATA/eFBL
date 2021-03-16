# eFBL Schema

```txt
https://fiata.com/digital/schemas/json/efbl.schema.json
```

electronic FIATA Bill of Lading

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [efbl.schema.json](../tooling/out/efbl.schema.json "open original schema") |

## eFBL Type

`object` ([eFBL](efbl.md))

# eFBL Properties

| Property                                              | Type     | Required | Nullable       | Defined by                                                                                                                                                          |
| :---------------------------------------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [exchanged_document](#exchanged_document)             | `object` | Optional | cannot be null | [eFBL](exchanged-document.md "https://fiata.com/digital/schemas/json/definitions/exchanged-document.schema.json#/properties/exchanged_document")                    |
| [supply_chain_consighment](#supply_chain_consighment) | `object` | Required | cannot be null | [eFBL](supply-chain-consignment.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/supply_chain_consighment") |

## exchanged_document

Exchanged Document

`exchanged_document`

*   is optional

*   Type: `object` ([Exchanged Document](exchanged-document.md))

*   cannot be null

*   defined in: [eFBL](exchanged-document.md "https://fiata.com/digital/schemas/json/definitions/exchanged-document.schema.json#/properties/exchanged_document")

### exchanged_document Type

`object` ([Exchanged Document](exchanged-document.md))

## supply_chain_consighment

A supply chain consignment specified for a use of this master message assembly.

`supply_chain_consighment`

*   is required

*   Type: `object` ([Supply Chain Consignment](supply-chain-consignment.md))

*   cannot be null

*   defined in: [eFBL](supply-chain-consignment.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/supply_chain_consighment")

### supply_chain_consighment Type

`object` ([Supply Chain Consignment](supply-chain-consignment.md))
