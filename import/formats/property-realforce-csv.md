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
| 10 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price per SQM |
| 11 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property habitable area |
| 12 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property land area |
| 13 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property number of rooms |
| 14 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property number of bedrooms |
| 15 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property number of bathrooms |
| 16 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property number of floors |
| 17 | string | [Property Availability](../values/property_availability_id.md) | Property availability |
| 18 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Promotion ID |
| 19 | string | [Transaction Type](../values/transaction_type_id.md) | Property transaction type |
| 20 | date | d.m.Y | d-m-Y | Y-m-d |  |
| 21 | json | { "location_path": LocationPath, "zip": string, "line1": string, "line2": string, "line3": string, "environmentId": string, "altitude": string, "longitude": string, "latitude": string } | Property real location |
| 22 | json | { "location_path": LocationPath, "zip": string, "line1": string, "line2": string, "line3": string, "environmentId": string, "altitude": string, "longitude": string, "latitude": string } | Property alternate location |
| 23 | json | { "filename": string, "brochure_page"?: 0|0.5|1, "is_website"?: boolean, "is_portal"?: boolean, "is_plan"?: boolean } | Semicolon separated list of photos |
| 24 | json | { "filename": string, "is_brochure"?: boolean, "is_plan"?: boolean } | Semicolon separated list of documents |

## Sample

[property-realforce.csv](../samples/property-realforce.csv)
```
ID,reference,statusId,categoryId,subcategoryId,price,currencyId,brokerAccountId,visibilityId,priceSqm,habitable,land,rooms,bedrooms,bathrooms,floors,availabilityId,promotionId,transactionTypeId,availabilityDate,realLocation,altLocation,photos,documents
OLDID00044,referenceTest,Actif,Appartement,Appartement à rénover,1200000,CHF,IDUSER001,Agence,1300,5000,15000,18,9,4,5,Immédiatement,,Vente,2022-08-31,"{""country"":""Suisse"",""canton"":""Genève"",""district"":""Aigle"",""zone"":""Genève"",""city"":""Genève"",""quarter"":""Champel"",""zip"":""1207"",""line1"":""Rue de la gare 1"",""line2"":""Les bureaux du futur"",""line3"":""Batiment A"",""environmentId"":""Montagne"",""altitude"":""1207"",""longitude"":""1207"",""latitude"":""1207""}","{""country"":""Suisse"",""canton"":""Genève"",""district"":""Aigle"",""zone"":""Genève"",""city"":""Genève"",""quarter"":""Champel"",""zip"":""1207"",""line1"":""Rue de la gare 1"",""line2"":""Les bureaux du futures"",""line3"":""Batiment A"",""environmentId"":""Ville"",""altitude"":""1207"",""longitude"":""1207"",""latitude"":""1207""}","{""filename"":""23849.jpg"",""brochure_page"":""1"",""is_plan"":""true"",""is_portal"":""true"",""is_website"":""true""};{""filename"":""23718.jpg"",""brochure_page"":""0.5"",""is_plan"":""false"",""is_portal"":""true"",""is_website"":""false""};{""filename"":""19571.jpg"",""brochure_page"":""0"",""is_plan"":""false"",""is_portal"":""false"",""is_website"":""true""};{""filename"":""23959.jpg"",""brochure_page"":""0"",""is_plan"":""false"",""is_portal"":""false"",""is_website"":""false""}",
```
