# Promotion - Realforce CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User ID in your system |
| 2 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | @rfDoc#ignore STRING instead of FOREIGN KEY because it is system generated instead of imported |
| 3 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Promotion reference |
| 5 | string | [Visibility](../values/visibility_id.md) | Promotion visibility/sharing |
| 6 | string | [Promotion Status](../values/promotion_status_id.md) | Promotion status |
| 7 | json | { "location_path": LocationPath, "zip": string, "line1": string, "line2": string, "line3": string, "environmentId": string, "altitude": string, "longitude": string, "latitude": string } | Real location for promotion |
| 8 | json | { "location_path": LocationPath, "zip": string, "line1": string, "line2": string, "line3": string, "environmentId": string, "altitude": string, "longitude": string, "latitude": string } | Alt location for promotion |

## Sample

[promotion-realforce.csv](../samples/promotion-realforce.csv)
```
ID,name,brokerAccountId,reference,visibilityId,StatusId,realLocation,altLocation
OLDID00044,Nouvelle promotion35,IDUSER001,EMS-35,132,342,"{""country"":""Suisse"",""canton"":""Genève"",""district"":""Aigle"",""zone"":""Genève"",""city"":""Genève"",""quarter"":""Champel"",""zip"":""1207"",""line1"":""Rue de la gare 1"",""line2"":""Les bureaux du futur"",""line3"":""Batiment A"",""environmentId"":""25"",""altitude"":""1207"",""longitude"":""1207"",""latitude"":""1207""}","{""country"":""Suisse"",""canton"":""Genève"",""district"":""Aigle"",""zone"":""Genève"",""city"":""Genève"",""quarter"":""Champel"",""zip"":""1207"",""line1"":""Rue de la gare 1"",""line2"":""Les bureaux du futures"",""line3"":""Batiment A"",""environmentId"":""25"",""altitude"":""1207"",""longitude"":""1207"",""latitude"":""1207""}"
```
