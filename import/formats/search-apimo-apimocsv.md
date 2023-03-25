# Search - Apimo APIMOCSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search ID in your system |
| 1 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Contact ID this search is linked to |
| 7 | string | [Search Transaction Type](../values/search_transaction_type_id.md) | Property transaction type |
| 8 | string | [Property Category](../values/property_category_id.md) | Property category |
| 8 | string | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 9 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price min |
| 10 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price max |
| 12 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room min |
| 12 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property bedroom min |
| 8,13 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property area min |
| 14 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property area max |
| 8,13 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property land min |
| 8,14 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property land max |
| 14 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Search real location |
| 18 | date | d.m.Y | d-m-Y | Y-m-d | Search update date |
| 19,39 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search private comment |
| 22 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |

## Sample

[search-apimo.apimocsv](../samples/search-apimo.apimocsv)
```

```
