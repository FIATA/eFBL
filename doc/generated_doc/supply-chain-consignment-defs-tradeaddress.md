# Untitled object in Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress
```



| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json*](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## tradeAddress Type

`object` ([Details](supply-chain-consignment-defs-tradeaddress.md))

# tradeAddress Properties

| Property                                          | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                                                   |
| :------------------------------------------------ | :------------ | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                                         | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-id.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/id")                                         |
| [postcode](#postcode)                             | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-postcode.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/postcode")                             |
| [streetName](#streetname)                         | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-streetname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/streetName")                         |
| [cityName](#cityname)                             | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-cityname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/cityName")                             |
| [countryCode](#countrycode)                       | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-country-code.md "https://fiata.com/digital/schemas/json/definitions/classes/country-code.schema.json#/$defs/tradeAddress/properties/countryCode")                           |
| [countryName](#countryname)                       | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-countryname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/countryName")                       |
| [countrySubDivisionName](#countrysubdivisionname) | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-countrysubdivisionname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/countrySubDivisionName") |

## id

A unique identifier of this trade address.

`id`

*   is optional

*   Type: `object[]` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-id.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/id")

### id Type

`object[]` ([Standardized Identifier](standardized-identifier.md))

## postcode

A code specifying the postcode of this trade address.

`postcode`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-postcode.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/postcode")

### postcode Type

`string`

## streetName

A name, expressed as text, of a street or thoroughfare for this trade address.

`streetName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-streetname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/streetName")

### streetName Type

`string`

## cityName

The name, expressed as text, of the city, town or village of this trade address.

`cityName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-cityname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/cityName")

### cityName Type

`string`

## countryCode

The unique identifier of a country for this trade address.

`countryCode`

*   is optional

*   Type: unknown ([Country Code](supply-chain-consignment-defs-tradeaddress-properties-country-code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-country-code.md "https://fiata.com/digital/schemas/json/definitions/classes/country-code.schema.json#/$defs/tradeAddress/properties/countryCode")

### countryCode Type

unknown ([Country Code](supply-chain-consignment-defs-tradeaddress-properties-country-code.md))

## countryName

A name, expressed as text, of the country for this trade address.

`countryName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-countryname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/countryName")

### countryName Type

`string`

## countrySubDivisionName

A name, expressed as text, of the sub-division of a country for this trade address.

`countrySubDivisionName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-countrysubdivisionname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/countrySubDivisionName")

### countrySubDivisionName Type

`string`
