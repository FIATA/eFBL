# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/paymentPlace
```

The location of the place of payment of this logistics service charge.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## paymentPlace Type

`object` ([Details](supply-chain-consignment-defs-paymentplace.md))

# paymentPlace Properties

| Property      | Type     | Required | Nullable       | Defined by                                                                                                                                                                                |
| :------------ | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)     | `object` | Optional | cannot be null | [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/paymentPlace/properties/id") |
| [name](#name) | `object` | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/paymentPlace/properties/name")                                     |

## id

Identifier which identification scheme is maintained by an external agency

`id`

*   is optional

*   Type: `object` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/paymentPlace/properties/id")

### id Type

`object` ([Standardized Identifier](standardized-identifier.md))

## name

The text with optional localization.

`name`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/paymentPlace/properties/name")

### name Type

`object` ([Text](text.md))
