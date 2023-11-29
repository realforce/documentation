# Property - Garaio IDX

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 6,7,8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ID in your system |
| 6,7,8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property reference |
| 3 | string | [Property Category](../values/property_category_id.md) | Property category |
| 3,4 |  | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 5,19,20 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price |
| 21 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property monthly charges |
| 23 | string | [Currency](../values/currency_id.md) | Property currency |
| 80 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 28 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property habitable area |
| 29 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land area |
| 30 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property usable area |
| 26 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of rooms |
| 16 | string | [Property Availability](../values/property_availability_id.md) | Property availability |
| 5 | string | [Property Transaction Type](../values/property_transaction_type_id.md) | Property transaction type |
| 16 | date | d.m.Y | d-m-Y | Y-m-d | Property availability date |
| 9,10,11 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Property real location |
| 9,10,11 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Property alternate location |
| 65 | json | { "filename": string, "is_brochure"?: boolean, "is_plan"?: boolean } | Semicolon separated list of documents |
| 47,48,49,50,51,88,89,90,91,143,144,145,146 | json | { "filename": string, "brochure_page"?: 0|0.5|1, "is_website"?: boolean, "is_portal"?: boolean, "is_plan"?: boolean } | Semicolon separated list of photos |
| 25 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property floor |
| 31 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property volume |
| 34,35,36,37,38,39,40,41,42,43,45,109,116,117,120,123,169,175 | json | { "amenity_id": string, "amenity_value": string } | amenities |
| 17 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property title |
| 18 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property description |
| 32 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year build |
| 110 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ceiling height |
| 163 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of floors |
| 164 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year renovated |
| 171 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is new |
| 181 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property visit3d |

## Sample

[property-garaio.idx](../samples/property-garaio.idx)
```

```
