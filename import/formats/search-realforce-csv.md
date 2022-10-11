# Search - Realforce CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search ID in your system |
| 2 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 3 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Contact ID this search is linked to |
| 4 | string | [Search Status](../values/search_status_id.md) | Search status |
| 5 | string | [Transaction Type](../values/transaction_type_id.md) | Property transaction type |
| 6 | string | [Property Category](../values/property_category_id.md) | Property category |
| 7 | string | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 8 | string | [Property Position](../values/property_position_id.md) | Semicolon separated list of property positions |
| 9 | string | [Property Furnishing](../values/property_furnishing_id.md) | Semicolon separated list of property furnishings |
| 10 | string | [Property Style](../values/property_style_id.md) | Semicolon separated list of property styles |
| 11 | string | [Property View](../values/property_view_id.md) | Semicolon separated list of property views |
| 12 | string | [Property Sonority](../values/property_sonority_id.md) | Semicolon separated list of property sonorities |
| 13 | string | [Property Space Type](../values/property_space_type_id.md) | Semicolon separated list of property space types |
| 14 | string | [Country](../values/country_id.md) | Semicolon separated list of property countries |
| 15 | string | [Canton](../values/canton_id.md) | Semicolon separated list of property cantons |
| 16 | string | [District](../values/district_id.md) | Semicolon separated list of property districts |
| 17 | string | [Zone](../values/zone_id.md) | Semicolon separated list of property zones |
| 18 | string | [City](../values/city_id.md) | Semicolon separated list of property cities |
| 19 | string | [Quarter](../values/quarter_id.md) | Semicolon separated list of property quarters |
| 20 | string | [Zip](../values/zip_id.md) | Semicolon separated list of property zipcodes |
| 21 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search label |
| 22 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search private comment |
| 23 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price min |
| 24 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price max |
| 25 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property area min |
| 26 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property area max |
| 27 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property room min |
| 28 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property room max |
| 29 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property bedroom min |
| 30 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property bedroom max |
| 31 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property land min |
| 32 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property land max |
| 33 | date | YYYY-MM-DD | Search update date |
| 34 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is new |
| 35 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is allowed to foreigners |
| 36 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Search is hidden in matching |

## Sample

[search-realforce.csv](../samples/search-realforce.csv)
```
ID,managerAccountId,contactContactId,statusId,transactionTypeId,categoryId,subcategoryId,positionIds,furnishingIds,styleIds,viewIds,sonorityIds,propertySpaceTypeIds,countryIds,cantonIds,districtIds,zoneIds,cityIds,quarterIds,zipIds,label,comment,priceMin,priceMax,areaMin,areaMax,roomMin,roomMax,bedroomMin,bedroomMax,landMin,landMax,updateDate,isPropertyNew,isAllowedForeigners,isHiddenMatching
IDSEARCH00001,IDUSER002,IDCONTACT000002,En cours,Location,Appartement,Appartement à rénover,Combles; Dernier étage,Non meublé; Meublé,Rustique; Classique,Aperçu; Belle vue; Campagne,Bruyant; Normal,Abri(s) de jardin; Arcade(s); Balcon(s),Suisse,Genève; Jura,Aigle,Broye-Vully,Genève; La Praille,Champel; Eaux-Vives,1201; 1001,Recherche importée de test,Ceci est un commentaire de test,1000,2000,100,200,3,4,1,2,1000,2000,2022-07-01,FALSE,TRUE,FALSE
```
