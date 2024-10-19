# Promotion - Imomig CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User ID in your system |
| 2 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | @rfDoc#ignore STRING instead of FOREIGN KEY because it is system generated instead of imported |
| 3 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Promotion reference |
| 5 | string | [Visibility](../values/visibility_id.md) | Promotion visibility/sharing |
| 14 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is archived |
| 6 | string | [Promotion Status](../values/promotion_status_id.md) | Promotion status |
| 22,23,24 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Promotion real location |
| 54 | json | { "filename": string, "brochure_page"?: 0|0.5|1, "is_website"?: boolean, "is_portal"?: boolean, "is_plan"?: boolean } | Semicolon separated list of photos |
| 160 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Promotion title |
| 161 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Promotion description |
| 161 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Promotion location description |

## Sample

[promotion-imomig.csv](../samples/promotion-imomig.csv)
```

```
