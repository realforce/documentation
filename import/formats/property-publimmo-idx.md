# Property - Publimmo IDX

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ID in your system |
| 6,7,8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property reference |
| 3 | string | [Property Category](../values/property_category_id.md) | Property category |
| 2,3 | string | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 5,19,20 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price |
| 23 | string | [Currency](../values/currency_id.md) | Property currency |
| 28,29,30 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property habitable area |
| 26 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property number of rooms |
| 163 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property number of floors |
| 16 | string | [Property Availability](../values/property_availability_id.md) | Property availability |
| 18 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Promotion ID |
| 5 | string | [Transaction Type](../values/transaction_type_id.md) | Property transaction type |
| 16 | date | d.m.Y | d-m-Y | Y-m-d |  |
| 9,10,11,12,13 | json | { "location_path": LocationPath, "zip": string, "line1": string, "line2": string, "line3": string, "environmentId": string, "altitude": string, "longitude": string, "latitude": string } | Property real location |
| 9,10,11,12,13 | json | { "location_path": LocationPath, "zip": string, "line1": string, "line2": string, "line3": string, "environmentId": string, "altitude": string, "longitude": string, "latitude": string } | Property alternate location |
| 25 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property floor |
| 31 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property volume |
| 34,35,36,37,38,39,40,41,42,43,45,109,116,117,120,123,169,175 | json | { "amenity_id": string, "value": string } | Property availability date |
| 17 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property title |
| 18 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property description |
| 32 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year build |
| 164 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year renovated |
| 110 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property ceiling height |
| 171 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | property is new |

## Sample

[property-publimmo.idx](../samples/property-publimmo.idx)
```

```
