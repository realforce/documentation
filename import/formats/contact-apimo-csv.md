# Contact - Apimo CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact ID in your system |
| 3 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 5 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact company name |
| 6,18 | string | [Contact Title](../values/contact_title_id.md) | Contact title |
| 7,19 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact lastname |
| 8,20 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact firstname |
| 10,22,41 | json | { "notes": string, "value": string, "is_use_mailing": boolean, "is_main": boolean } | Semicolon separated list of emails |
| 11,12,23 | json | { "notes": string, "number": string, "type": mobile/landline, "is_main": boolean } | Semicolon separated list of phones |
| 14 | date | d.m.Y | d-m-Y | Y-m-d | Contact birthdate |
| 16,26,32 | string | [Country](../values/country_id.md) | Contact nationality |
| 32,28,29,31,30 | json | { "notes": string, "country_id": string, "line1": string, "line2": string, "line3": string, "city": string, "zip": string, "use_default": boolean } | Semicolon separated list of addresses |
| 33,35,37,38,42 | string | [Contact Type](../values/contact_type_id.md) | Semicolon separated list of contact types |
| 44,45 | string | [Language](../values/language_id.md) | Contact language |
| 53 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Contact creation date & time |
| 54 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Contact update date & time |
| 55 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact private comment |
| 24 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the sale broker in charge |
| 34,36 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is archived |

## Sample

[contact-apimo.csv](../samples/contact-apimo.csv)
```

```
