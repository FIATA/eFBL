# Supply Chain Consignment Schema

```txt
https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json
```

A supply chain consignment specified for a use of this master message assembly.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                     |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [supply-chain-consignment.schema.json](../tooling/out/definitions/supply-chain-consignment.schema.json "open original schema") |

## Supply Chain Consignment Type

`object` ([Supply Chain Consignment](supply-chain-consignment.md))

# Supply Chain Consignment Properties

| Property                                                          | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                            |
| :---------------------------------------------------------------- | :------------ | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [totalChargeAmount](#totalchargeamount)                           | `object`      | Optional | cannot be null | [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/properties/totalChargeAmount")                                                                                   |
| [cargoInsuranceNotProvidedByCTO](#cargoinsurancenotprovidedbycto) | `boolean`     | Optional | cannot be null | [Supply Chain Consignment](indicator.md "https://fiata.com/digital/schemas/json/definitions/indicator.schema.json#/properties/cargoInsuranceNotProvidedByCTO")                                                                        |
| [numberOfPackages](#numberofpackages)                             | `number`      | Optional | cannot be null | [Supply Chain Consignment](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/numberOfPackages")                                                                                      |
| [declaredValueForCarriageAmount](#declaredvalueforcarriageamount) | `object`      | Optional | cannot be null | [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/properties/declaredValueForCarriageAmount")                                                                      |
| [consignor](#consignor)                                           | `object`      | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/consignor")                                              |
| [consignee](#consignee)                                           | `object`      | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/consignee")                                              |
| [cto](#cto)                                                       | `object`      | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/cto")                                                    |
| [ctoAgent](#ctoagent)                                             | `object`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/ctoAgent")                                               |
| [notifiedParty](#notifiedparty)                                   | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-properties-notifiedparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/notifiedParty")                                 |
| [carrierAcceptanceLocation](#carrieracceptancelocation)           | Not specified | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-properties-carrieracceptancelocation.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/carrierAcceptanceLocation")         |
| [consigneeReceiptLocation](#consigneereceiptlocation)             | Not specified | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-properties-consigneereceiptlocation.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/consigneeReceiptLocation")           |
| [loadingBaseportLocation](#loadingbaseportlocation)               | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-properties-loadingbaseportlocation.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/loadingBaseportLocation")             |
| [unloadingBaseportLocation](#unloadingbaseportlocation)           | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-properties-unloadingbaseportlocation.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/unloadingBaseportLocation")         |
| [includedConsignmentItem](#includedconsignmentitem)               | `array`       | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-properties-includedconsignmentitem.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/includedConsignmentItem")             |
| [mainCarriageTransportMovement](#maincarriagetransportmovement)   | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-properties-maincarriagetransportmovement.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/mainCarriageTransportMovement") |
| [applicableServiceCharge](#applicableservicecharge)               | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-properties-applicableservicecharge.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/applicableServiceCharge")             |

## totalChargeAmount

A number of monetary units specified in a currency where the unit of the currency is explicit or implied.

`totalChargeAmount`

*   is optional

*   Type: `object` ([Amount](amount.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/properties/totalChargeAmount")

### totalChargeAmount Type

`object` ([Amount](amount.md))

## cargoInsuranceNotProvidedByCTO

An indicator with true/false, yes/no value

`cargoInsuranceNotProvidedByCTO`

*   is optional

*   Type: `boolean` ([Indicator](indicator.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](indicator.md "https://fiata.com/digital/schemas/json/definitions/indicator.schema.json#/properties/cargoInsuranceNotProvidedByCTO")

### cargoInsuranceNotProvidedByCTO Type

`boolean` ([Indicator](indicator.md))

## numberOfPackages

A counted number of non-monetary units possibly including fractions.

`numberOfPackages`

*   is optional

*   Type: `number` ([Identifier](quantity.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/properties/numberOfPackages")

### numberOfPackages Type

`number` ([Identifier](quantity.md))

## declaredValueForCarriageAmount

A number of monetary units specified in a currency where the unit of the currency is explicit or implied.

`declaredValueForCarriageAmount`

*   is optional

*   Type: `object` ([Amount](amount.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/properties/declaredValueForCarriageAmount")

### declaredValueForCarriageAmount Type

`object` ([Amount](amount.md))

## consignor

The consignor party for this supply chain consignment.

`consignor`

*   is required

*   Type: `object` ([Details](supply-chain-consignment-defs-tradeparty.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/consignor")

### consignor Type

`object` ([Details](supply-chain-consignment-defs-tradeparty.md))

## consignee

The consignee party for this supply chain consignment.

`consignee`

*   is required

*   Type: `object` ([Details](supply-chain-consignment-defs-tradeparty.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/consignee")

### consignee Type

`object` ([Details](supply-chain-consignment-defs-tradeparty.md))

## cto

The carrier party for this supply chain consignment.

`cto`

*   is required

*   Type: `object` ([Details](supply-chain-consignment-defs-tradeparty.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/cto")

### cto Type

`object` ([Details](supply-chain-consignment-defs-tradeparty.md))

## ctoAgent

The party acting as the agent of the carrier for this supply chain consignment.

`ctoAgent`

*   is optional

*   Type: `object` ([Details](supply-chain-consignment-defs-tradeparty.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/ctoAgent")

### ctoAgent Type

`object` ([Details](supply-chain-consignment-defs-tradeparty.md))

## notifiedParty

A party who has been or will be notified about this supply chain consignment.

`notifiedParty`

*   is optional

*   Type: `object[]` ([Details](supply-chain-consignment-defs-tradeparty.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-properties-notifiedparty.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/notifiedParty")

### notifiedParty Type

`object[]` ([Details](supply-chain-consignment-defs-tradeparty.md))

## carrierAcceptanceLocation

The location where this supply chain consignment will be, or has been, accepted by the carrier.

`carrierAcceptanceLocation`

*   is required

*   Type: unknown

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-properties-carrieracceptancelocation.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/carrierAcceptanceLocation")

### carrierAcceptanceLocation Type

unknown

## consigneeReceiptLocation

The location at which this supply chain consignment will be or has been received by the consignee.

`consigneeReceiptLocation`

*   is required

*   Type: unknown

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-properties-consigneereceiptlocation.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/consigneeReceiptLocation")

### consigneeReceiptLocation Type

unknown

## loadingBaseportLocation

The baseport location at which this supply chain consignment is to be loaded on a means of transport according to the transport contract.

`loadingBaseportLocation`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-properties-loadingbaseportlocation.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/loadingBaseportLocation")

### loadingBaseportLocation Type

unknown

## unloadingBaseportLocation

The baseport location at which this supply chain consignment is to be unloaded from a means of transport according to the transport contract.

`unloadingBaseportLocation`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-properties-unloadingbaseportlocation.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/unloadingBaseportLocation")

### unloadingBaseportLocation Type

unknown

## includedConsignmentItem

A consignment item included in this supply chain consignment.

`includedConsignmentItem`

*   is required

*   Type: unknown\[]

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-properties-includedconsignmentitem.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/includedConsignmentItem")

### includedConsignmentItem Type

unknown\[]

### includedConsignmentItem Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

## mainCarriageTransportMovement

A main carriage logistics transport movement for this supply chain consignment.

`mainCarriageTransportMovement`

*   is optional

*   Type: `object[]` ([Details](supply-chain-consignment-defs-logisticstransportmeans.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-properties-maincarriagetransportmovement.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/mainCarriageTransportMovement")

### mainCarriageTransportMovement Type

`object[]` ([Details](supply-chain-consignment-defs-logisticstransportmeans.md))

## applicableServiceCharge

A logistics service charge applicable to this supply chain consignment, such as freight or insurance charges.

`applicableServiceCharge`

*   is optional

*   Type: `object[]` ([Details](supply-chain-consignment-defs-paymentplace.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-properties-applicableservicecharge.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/properties/applicableServiceCharge")

### applicableServiceCharge Type

`object[]` ([Details](supply-chain-consignment-defs-paymentplace.md))

# Supply Chain Consignment Definitions

## Definitions group tradeParty

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty"}
```

| Property                                          | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                               |
| :------------------------------------------------ | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                                         | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-id.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/id")                                         |
| [name](#name)                                     | `object` | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/tradeParty/properties/name")                                                                                                      |
| [languageCode](#languagecode)                     | `object` | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/tradeParty/properties/languageCode")                                                                                              |
| [definedContactDetails](#definedcontactdetails)   | `object` | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/definedContactDetails")                                  |
| [postalAddress](#postaladdress)                   | `object` | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/postalAddress")                                          |
| [taxRegistration](#taxregistration)               | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-taxregistration.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/taxRegistration")               |
| [governmentRegistration](#governmentregistration) | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-governmentregistration.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/governmentRegistration") |

### id

A unique identifier of this trade party.

`id`

*   is optional

*   Type: `object[]` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-id.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/id")

#### id Type

`object[]` ([Standardized Identifier](standardized-identifier.md))

### name

The text with optional localization.

`name`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/tradeParty/properties/name")

#### name Type

`object` ([Text](text.md))

### languageCode

A code.

`languageCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/tradeParty/properties/languageCode")

#### languageCode Type

`object` ([Code](code.md))

### definedContactDetails

A trade contact defined for this trade party.

`definedContactDetails`

*   is optional

*   Type: `object` ([Details](supply-chain-consignment-defs-tradecontact.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/definedContactDetails")

#### definedContactDetails Type

`object` ([Details](supply-chain-consignment-defs-tradecontact.md))

### postalAddress

The postal address for this trade party.

`postalAddress`

*   is optional

*   Type: `object` ([Details](supply-chain-consignment-defs-tradeaddress.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/postalAddress")

#### postalAddress Type

`object` ([Details](supply-chain-consignment-defs-tradeaddress.md))

### taxRegistration

A tax registration specified for this trade party.

`taxRegistration`

*   is optional

*   Type: `object[]` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-taxregistration.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/taxRegistration")

#### taxRegistration Type

`object[]` ([Standardized Identifier](standardized-identifier.md))

### governmentRegistration

A governmental registration specified for this trade party.

`governmentRegistration`

*   is optional

*   Type: `object[]` ([Details](supply-chain-consignment-defs-governmentregistration.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeparty-properties-governmentregistration.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeParty/properties/governmentRegistration")

#### governmentRegistration Type

`object[]` ([Details](supply-chain-consignment-defs-governmentregistration.md))

## Definitions group tradeContact

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeContact"}
```

| Property                            | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                                     |
| :---------------------------------- | :------------ | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [personName](#personname)           | `object`      | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/tradeContact/properties/personName")                                                                                    |
| [telephone](#telephone)             | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-complete-number.md "https://fiata.com/digital/schemas/json/definitions/classes/complete-number.schema.json#/$defs/tradeContact/properties/telephone")         |
| [mobileTelephone](#mobiletelephone) | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-complete-number-1.md "https://fiata.com/digital/schemas/json/definitions/classes/complete-number.schema.json#/$defs/tradeContact/properties/mobileTelephone") |
| [emailAddress](#emailaddress)       | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-uri.md "https://fiata.com/digital/schemas/json/definitions/classes/uri.schema.json#/$defs/tradeContact/properties/emailAddress")                              |
| [note](#note)                       | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-note.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeContact/properties/note")                       |

### personName

The text with optional localization.

`personName`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/tradeContact/properties/personName")

#### personName Type

`object` ([Text](text.md))

### telephone

Telephone communication information for this trade contact.

`telephone`

*   is optional

*   Type: unknown ([Complete Number](supply-chain-consignment-defs-tradecontact-properties-complete-number.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-complete-number.md "https://fiata.com/digital/schemas/json/definitions/classes/complete-number.schema.json#/$defs/tradeContact/properties/telephone")

#### telephone Type

unknown ([Complete Number](supply-chain-consignment-defs-tradecontact-properties-complete-number.md))

### mobileTelephone

The mobile telephone communication information for this trade contact.

`mobileTelephone`

*   is optional

*   Type: unknown ([Complete Number](supply-chain-consignment-defs-tradecontact-properties-complete-number-1.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-complete-number-1.md "https://fiata.com/digital/schemas/json/definitions/classes/complete-number.schema.json#/$defs/tradeContact/properties/mobileTelephone")

#### mobileTelephone Type

unknown ([Complete Number](supply-chain-consignment-defs-tradecontact-properties-complete-number-1.md))

### emailAddress

The email URI communication information for this trade contact.

`emailAddress`

*   is optional

*   Type: unknown ([URI](supply-chain-consignment-defs-tradecontact-properties-uri.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-uri.md "https://fiata.com/digital/schemas/json/definitions/classes/uri.schema.json#/$defs/tradeContact/properties/emailAddress")

#### emailAddress Type

unknown ([URI](supply-chain-consignment-defs-tradecontact-properties-uri.md))

### note

A note specified for this trade contact.

`note`

*   is optional

*   Type: `object[]` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradecontact-properties-note.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeContact/properties/note")

#### note Type

`object[]` ([Text](text.md))

## Definitions group tradeAddress

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress"}
```

| Property                                          | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                                                   |
| :------------------------------------------------ | :------------ | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id-1)                                       | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-id.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/id")                                         |
| [postcode](#postcode)                             | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-postcode.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/postcode")                             |
| [streetName](#streetname)                         | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-streetname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/streetName")                         |
| [cityName](#cityname)                             | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-cityname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/cityName")                             |
| [countryCode](#countrycode)                       | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-country-code.md "https://fiata.com/digital/schemas/json/definitions/classes/country-code.schema.json#/$defs/tradeAddress/properties/countryCode")                           |
| [countryName](#countryname)                       | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-countryname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/countryName")                       |
| [countrySubDivisionName](#countrysubdivisionname) | `string`      | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-countrysubdivisionname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/countrySubDivisionName") |

### id

A unique identifier of this trade address.

`id`

*   is optional

*   Type: `object[]` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-id.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/id")

#### id Type

`object[]` ([Standardized Identifier](standardized-identifier.md))

### postcode

A code specifying the postcode of this trade address.

`postcode`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-postcode.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/postcode")

#### postcode Type

`string`

### streetName

A name, expressed as text, of a street or thoroughfare for this trade address.

`streetName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-streetname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/streetName")

#### streetName Type

`string`

### cityName

The name, expressed as text, of the city, town or village of this trade address.

`cityName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-cityname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/cityName")

#### cityName Type

`string`

### countryCode

The unique identifier of a country for this trade address.

`countryCode`

*   is optional

*   Type: unknown ([Country Code](supply-chain-consignment-defs-tradeaddress-properties-country-code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-country-code.md "https://fiata.com/digital/schemas/json/definitions/classes/country-code.schema.json#/$defs/tradeAddress/properties/countryCode")

#### countryCode Type

unknown ([Country Code](supply-chain-consignment-defs-tradeaddress-properties-country-code.md))

### countryName

A name, expressed as text, of the country for this trade address.

`countryName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-countryname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/countryName")

#### countryName Type

`string`

### countrySubDivisionName

A name, expressed as text, of the sub-division of a country for this trade address.

`countrySubDivisionName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-tradeaddress-properties-countrysubdivisionname.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/tradeAddress/properties/countrySubDivisionName")

#### countrySubDivisionName Type

`string`

## Definitions group governmentRegistration

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/governmentRegistration"}
```

| Property                      | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                                             |
| :---------------------------- | :------------ | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id-2)                   | `object`      | Optional | cannot be null | [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/governmentRegistration/properties/id")                                                    |
| [typeCode](#typecode)         | `object`      | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/governmentRegistration/properties/typeCode")                                                                                    |
| [countryCode](#countrycode-1) | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-governmentregistration-properties-country-code.md "https://fiata.com/digital/schemas/json/definitions/classes/country-code.schema.json#/$defs/governmentRegistration/properties/countryCode") |

### id

Identifier which identification scheme is maintained by an external agency

`id`

*   is optional

*   Type: `object` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/governmentRegistration/properties/id")

#### id Type

`object` ([Standardized Identifier](standardized-identifier.md))

### typeCode

A code.

`typeCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/governmentRegistration/properties/typeCode")

#### typeCode Type

`object` ([Code](code.md))

### countryCode



`countryCode`

*   is optional

*   Type: unknown ([Country Code](supply-chain-consignment-defs-governmentregistration-properties-country-code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-governmentregistration-properties-country-code.md "https://fiata.com/digital/schemas/json/definitions/classes/country-code.schema.json#/$defs/governmentRegistration/properties/countryCode")

#### countryCode Type

unknown ([Country Code](supply-chain-consignment-defs-governmentregistration-properties-country-code.md))

## Definitions group consignmentItem

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem"}
```

| Property                                                            | Type          | Required | Nullable       | Defined by                                                                                                                                                                                                                                                           |
| :------------------------------------------------------------------ | :------------ | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [goodsTypeCode](#goodstypecode)                                     | `object`      | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/consignmentItem/properties/goodsTypeCode")                                                                                                    |
| [declaredValueForCarriageAmount](#declaredvalueforcarriageamount-1) | `object`      | Optional | cannot be null | [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/$defs/consignmentItem/properties/declaredValueForCarriageAmount")                                                                               |
| [insuranceValueAmount](#insurancevalueamount)                       | `object`      | Optional | cannot be null | [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/$defs/consignmentItem/properties/insuranceValueAmount")                                                                                         |
| [grossWeight](#grossweight)                                         | `object`      | Optional | cannot be null | [Supply Chain Consignment](measure.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/$defs/consignmentItem/properties/grossWeight")                                                                                                |
| [grossVolume](#grossvolume)                                         | `object`      | Optional | cannot be null | [Supply Chain Consignment](measure.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/$defs/consignmentItem/properties/grossVolume")                                                                                                |
| [cargoNatureIdentification](#cargonatureidentification)             | `object`      | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-transportcargo.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/cargoNatureIdentification")                                   |
| [transportDangerousGoods](#transportdangerousgoods)                 | `array`       | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-consignmentitem-properties-transportdangerousgoods.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportDangerousGoods") |
| [transportPackage](#transportpackage)                               | Not specified | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-consignmentitem-properties-transportpackage.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportPackage")               |

### goodsTypeCode

A code.

`goodsTypeCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/consignmentItem/properties/goodsTypeCode")

#### goodsTypeCode Type

`object` ([Code](code.md))

### declaredValueForCarriageAmount

A number of monetary units specified in a currency where the unit of the currency is explicit or implied.

`declaredValueForCarriageAmount`

*   is optional

*   Type: `object` ([Amount](amount.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/$defs/consignmentItem/properties/declaredValueForCarriageAmount")

#### declaredValueForCarriageAmount Type

`object` ([Amount](amount.md))

### insuranceValueAmount

A number of monetary units specified in a currency where the unit of the currency is explicit or implied.

`insuranceValueAmount`

*   is optional

*   Type: `object` ([Amount](amount.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](amount.md "https://fiata.com/digital/schemas/json/definitions/classes/amount.schema.json#/$defs/consignmentItem/properties/insuranceValueAmount")

#### insuranceValueAmount Type

`object` ([Amount](amount.md))

### grossWeight

A measure with its unit.

`grossWeight`

*   is optional

*   Type: `object` ([Measure](measure.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](measure.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/$defs/consignmentItem/properties/grossWeight")

#### grossWeight Type

`object` ([Measure](measure.md))

### grossVolume

A measure with its unit.

`grossVolume`

*   is optional

*   Type: `object` ([Measure](measure.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](measure.md "https://fiata.com/digital/schemas/json/definitions/classes/measure.schema.json#/$defs/consignmentItem/properties/grossVolume")

#### grossVolume Type

`object` ([Measure](measure.md))

### cargoNatureIdentification

Transport cargo details of this supply chain consignment item sufficient to identify its nature for customs, statistical or transport purposes.

`cargoNatureIdentification`

*   is required

*   Type: `object` ([Details](supply-chain-consignment-defs-transportcargo.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-transportcargo.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/cargoNatureIdentification")

#### cargoNatureIdentification Type

`object` ([Details](supply-chain-consignment-defs-transportcargo.md))

### transportDangerousGoods

Dangerous goods transport details applicable to this supply chain consignment item.

`transportDangerousGoods`

*   is optional

*   Type: `object[]` ([Details](supply-chain-consignment-defs-transportdangerouscode.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-consignmentitem-properties-transportdangerousgoods.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportDangerousGoods")

#### transportDangerousGoods Type

`object[]` ([Details](supply-chain-consignment-defs-transportdangerouscode.md))

### transportPackage

A transport package for this supply chain consignment item.

`transportPackage`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-consignmentitem-properties-transportpackage.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/consignmentItem/properties/transportPackage")

#### transportPackage Type

unknown

## Definitions group transportCargo

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/transportCargo"}
```

| Property                                  | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                               |
| :---------------------------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [typeCode](#typecode-1)                   | `object` | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/transportCargo/properties/typeCode")                                                                                              |
| [identificationText](#identificationtext) | `array`  | Required | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-transportcargo-properties-identificationtext.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/transportCargo/properties/identificationText") |

### typeCode

A code.

`typeCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/transportCargo/properties/typeCode")

#### typeCode Type

`object` ([Code](code.md))

### identificationText

Identification, expressed as text, of this transport cargo that is sufficient to identify it for customs, statistical or transport purposes.

`identificationText`

*   is required

*   Type: `object[]` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-transportcargo-properties-identificationtext.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/transportCargo/properties/identificationText")

#### identificationText Type

`object[]` ([Text](text.md))

#### identificationText Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

## Definitions group transportDangerousCode

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/transportDangerousCode"}
```

| Property                                          | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                              |
| :------------------------------------------------ | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [undgId](#undgid)                                 | `object` | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/transportDangerousCode/properties/undgId")                                                       |
| [hazardClassificationId](#hazardclassificationid) | `object` | Optional | cannot be null | [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/transportDangerousCode/properties/hazardClassificationId") |

### undgId

A code.

`undgId`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/transportDangerousCode/properties/undgId")

#### undgId Type

`object` ([Code](code.md))

### hazardClassificationId

Identifier which identification scheme is maintained by an external agency

`hazardClassificationId`

*   is optional

*   Type: `object` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/transportDangerousCode/properties/hazardClassificationId")

#### hazardClassificationId Type

`object` ([Standardized Identifier](standardized-identifier.md))

## Definitions group logisticsPackage

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage"}
```

| Property                        | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                         |
| :------------------------------ | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [itemQuantity](#itemquantity)   | `number` | Optional | cannot be null | [Supply Chain Consignment](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/$defs/logisticsPackage/properties/itemQuantity")                                                                                |
| [typeCode](#typecode-2)         | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-typecode.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/typeCode")           |
| [typeText](#typetext)           | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-typetext.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/typeText")           |
| [shippingMarks](#shippingmarks) | `array`  | Optional | cannot be null | [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-shippingmarks.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/shippingMarks") |

### itemQuantity

A counted number of non-monetary units possibly including fractions.

`itemQuantity`

*   is optional

*   Type: `number` ([Identifier](quantity.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](quantity.md "https://fiata.com/digital/schemas/json/definitions/identifier.schema.json#/$defs/logisticsPackage/properties/itemQuantity")

#### itemQuantity Type

`number` ([Identifier](quantity.md))

### typeCode

A code specifying the type of logistics package.

`typeCode`

*   is optional

*   Type: `object[]` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-typecode.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/typeCode")

#### typeCode Type

`object[]` ([Code](code.md))

### typeText

A type, expressed as text, of this logistics package.

`typeText`

*   is optional

*   Type: `object[]` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-typetext.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/typeText")

#### typeText Type

`object[]` ([Text](text.md))

### shippingMarks

Physical shipping marks and barcode information for this logistics package.

`shippingMarks`

*   is optional

*   Type: `object[]` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](supply-chain-consignment-defs-logisticspackage-properties-shippingmarks.md "https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsPackage/properties/shippingMarks")

#### shippingMarks Type

`object[]` ([Text](text.md))

## Definitions group logisticsTransportMeans

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/logisticsTransportMeans"}
```

| Property                | Type     | Required | Nullable       | Defined by                                                                                                                                                                                           |
| :---------------------- | :------- | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [typeCode](#typecode-3) | `object` | Optional | cannot be null | [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/logisticsTransportMeans/properties/typeCode")                                 |
| [typeText](#typetext-1) | `object` | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/logisticsTransportMeans/properties/typeText")                                 |
| [id](#id-3)             | `object` | Optional | cannot be null | [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/logisticsTransportMeans/properties/id") |
| [name](#name-1)         | `object` | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/logisticsTransportMeans/properties/name")                                     |

### typeCode

A code.

`typeCode`

*   is optional

*   Type: `object` ([Code](code.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](code.md "https://fiata.com/digital/schemas/json/definitions/classes/code.schema.json#/$defs/logisticsTransportMeans/properties/typeCode")

#### typeCode Type

`object` ([Code](code.md))

### typeText

The text with optional localization.

`typeText`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/logisticsTransportMeans/properties/typeText")

#### typeText Type

`object` ([Text](text.md))

### id

Identifier which identification scheme is maintained by an external agency

`id`

*   is optional

*   Type: `object` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/logisticsTransportMeans/properties/id")

#### id Type

`object` ([Standardized Identifier](standardized-identifier.md))

### name

The text with optional localization.

`name`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/logisticsTransportMeans/properties/name")

#### name Type

`object` ([Text](text.md))

## Definitions group paymentPlace

Reference this group by using

```json
{"$ref":"https://fiata.com/digital/schemas/json/definitions/suppliy-chain-consignment.schema.json#/$defs/paymentPlace"}
```

| Property        | Type     | Required | Nullable       | Defined by                                                                                                                                                                                |
| :-------------- | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id-4)     | `object` | Optional | cannot be null | [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/paymentPlace/properties/id") |
| [name](#name-2) | `object` | Optional | cannot be null | [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/paymentPlace/properties/name")                                     |

### id

Identifier which identification scheme is maintained by an external agency

`id`

*   is optional

*   Type: `object` ([Standardized Identifier](standardized-identifier.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](standardized-identifier.md "https://fiata.com/digital/schemas/json/definitions/classes/standardized-identifier.schema.json#/$defs/paymentPlace/properties/id")

#### id Type

`object` ([Standardized Identifier](standardized-identifier.md))

### name

The text with optional localization.

`name`

*   is optional

*   Type: `object` ([Text](text.md))

*   cannot be null

*   defined in: [Supply Chain Consignment](text.md "https://fiata.com/digital/schemas/json/definitions/classes/text.schema.json#/$defs/paymentPlace/properties/name")

#### name Type

`object` ([Text](text.md))
