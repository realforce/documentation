# Property - Realforce CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ID in your system |
| 2 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property reference |
| 3 | string | [Property Status](../values/property_status_id.md) | Property status |
| 4 | string | [Property Category](../values/property_category_id.md) | Property category |
| 5 | string | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 6 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price |
| 7 | string | [Currency](../values/currency_id.md) | Property currency |
| 8 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 9 | string | [Visibility](../values/visibility_id.md) | Property visibility/sharing |
| 10 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property priceqm |
| 11 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property habitable |
| 12 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property land |
| 13 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property rooms |
| 14 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property bedrooms |
| 15 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property bathrooms |
| 16 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property floors |
| 17 | string | [Property Availability](../values/property_availability_id.md) | Property availibility |
| 18 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Promotion ID |
| 19 | string | [Transaction Type](../values/transaction_type_id.md) | Property transaction type |
| 20 | date | YYYY-MM-DD | Property availability date |
| 21 | json | { "location_path": LocationPath, "zip": string, "line1": string, "line2": string, "line3": string, "environmentId": string, "altitude": string, "longitude": string, "latitude": string } | Real location for property |
| 22 | json | { "location_path": LocationPath, "zip": string, "line1": string, "line2": string, "line3": string, "environmentId": string, "altitude": string, "longitude": string, "latitude": string } | Alt location for property |

## Sample

[property-realforce.csv](../samples/property-realforce.csv)
```
ID,reference,statusId,categoryId,subcategoryId,price,currencyId,brokerAccountId,visibilityId,priceSqm,habitable,land,rooms,bedrooms,bathrooms,floors,availabilityId,promotionId,transactionTypeId,availabilityDate,realLocation,altLocation
OLDID00044,referenceTest,En cours,Appartement,Appartement à rénover,1200000,CHF,IDUSER001,Agence,1300,5000,15000,18,9,4,5,Immédiatement,2673,Vente,2022-08-31,"{""country"":""Suisse"",""canton"":""Genève"",""district"":""Aigle"",""zone"":""Genève"",""city"":""Genève"",""quarter"":""Champel"",""zip"":""1207"",""line1"":""Rue de la gare 1"",""line2"":""Les bureaux du futur"",""line3"":""Batiment A"",""environmentId"":""25"",""altitude"":""1207"",""longitude"":""1207"",""latitude"":""1207""}","{""country"":""Suisse"",""canton"":""Genève"",""district"":""Aigle"",""zone"":""Genève"",""city"":""Genève"",""quarter"":""Champel"",""zip"":""1207"",""line1"":""Rue de la gare 1"",""line2"":""Les bureaux du futures"",""line3"":""Batiment A"",""environmentId"":""25"",""altitude"":""1207"",""longitude"":""1207"",""latitude"":""1207""}"
```
