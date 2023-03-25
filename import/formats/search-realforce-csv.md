# Search - Realforce CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search ID in your system |
| 2 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 3 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Contact ID this search is linked to |
| 4 | string | [Search Status](../values/search_status_id.md) | Search status |
| 5 | string | [Search Transaction Type](../values/search_transaction_type_id.md) | Property transaction type |
| 6 | string | [Property Category](../values/property_category_id.md) | Property category |
| 7 | string | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 8 | string | [Property Position](../values/property_position_id.md) | Semicolon separated list of property positions |
| 9 | string | [Property Furnishing](../values/property_furnishing_id.md) | Semicolon separated list of property furnishings |
| 10 | string | [Property Style](../values/property_style_id.md) | Semicolon separated list of property styles |
| 11 | string | [Property View](../values/property_view_id.md) | Semicolon separated list of property views |
| 12 | string | [Property Sonority](../values/property_sonority_id.md) | Semicolon separated list of property sonorities |
| 13 | string | [Property Space Type](../values/property_space_type_id.md) | Semicolon separated list of property space types |
| 14 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Search real location |
| 15 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search label |
| 16 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search private comment |
| 17 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price min |
| 18 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price max |
| 19 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property area min |
| 20 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property area max |
| 21 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room min |
| 22 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room max |
| 23 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property bedroom min |
| 24 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property bedroom max |
| 25 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property land min |
| 26 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property land max |
| 27 | date | d.m.Y | d-m-Y | Y-m-d | Search update date |
| 28 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is new |
| 29 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is allowed to foreigners |
| 30 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Search is hidden in global matching |

## Sample

[search-realforce.csv](../samples/search-realforce.csv)
```
ID,managerAccountId,contactContactId,statusId,transactionTypeId,categoryId,subcategoryId,positionIds,furnishingIds,styleIds,viewIds,sonorityIds,propertySpaceTypeIds,realLocation,label,comment,priceMin,priceMax,areaMin,areaMax,roomMin,roomMax,bedroomMin,bedroomMax,landMin,landMax,updateDate,isPropertyNew,isAllowedForeigners,isHiddenMatching
IDSEARCH00001,IDUSER002,IDCONTACT000002,En cours,Location,Appartement,Appartement à rénover,Combles; Dernier étage,Non meublé; Meublé,Rustique; Classique,Aperçu; Belle vue; Campagne,Bruyant; Normal,Abri(s) de jardin; Arcade(s); Balcon(s),"{""location_name"":""geneve"", ""location_level"":""zone"", ""zip"":"""", ""line1"":"""", ""line2"":"""", ""line3"":"""", ""environment_id"":"""", ""altitude"":"""", ""longitude"":"""", ""latitude"":""""}; {""location_name"":""sion"", ""location_level"":""canton"", ""zip"":"""", ""line1"":"""", ""line2"":"""", ""line3"":"""", ""environment_id"":"""", ""altitude"":"""", ""longitude"":"""", ""latitude"":""""}",Recherche importée de test,Ceci est un commentaire de test,1000,2000,100,200,3,4,1,2,1000,2000,2022-07-01,FALSE,TRUE,FALSE
```
