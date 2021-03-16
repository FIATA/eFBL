# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/governmentRegistration
```

A governmental registration

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## governmentRegistration Type

`object` ([Details](supply-chain-consignment-defs-governmentregistration.md))

# governmentRegistration Properties

| Property                    | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                                             |
| :-------------------------- | :------------ | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                   | `object`      | Optional | cannot be null | [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/governmentRegistration/properties/id")                                                    |
| [typeCode](#typecode)       | `object`      | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/governmentRegistration/properties/typeCode")                                                                                    |
| [countryCode](#countrycode) | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-governmentregistration-properties-country-code.md "https://fiata.com/digital/schemas/json/definitions/classes/country-code.schema.json#/$defs/governmentRegistration/properties/countryCode") |

## id

Identifier which identification scheme is maintained by an external agency

`id`

*   is optional

*   Type: `object` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/governmentRegistration/properties/id")

### id Type

`object` ([Standardized Identifier](standardized-identifier.md))

## typeCode

A code.

`typeCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/governmentRegistration/properties/typeCode")

### typeCode Type

`object` ([Code](code.md))

## countryCode



`countryCode`

*   is optional

*   Type: unknown ([Country Code](supply-chain-consignment-defs-governmentregistration-properties-country-code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-governmentregistration-properties-country-code.md "https://fiata.com/digital/schemas/json/definitions/classes/country-code.schema.json#/$defs/governmentRegistration/properties/countryCode")

### countryCode Type

unknown ([Country Code](supply-chain-consignment-defs-governmentregistration-properties-country-code.md))
