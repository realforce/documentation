# Labels - Locations
Fetch "locations" labels linked to the public data you retrieve from the public API endpoints.

## Endpoint
```
GET https://labels.realforce.ch/api/v1/get-locations?is_country={is_country}&is_canton={is_canton}&is_district={is_district}&is_zone={is_zone}&is_city={is_city}&is_quarter={is_quarter}&country_id={country_id}&canton_id={canton_id}&district_id={district_id}&zone_id={zone_id}&city_id={city_id}&quarter_id={quarter_id}&lang={lang}
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Parameters

| Name        | Type   | Required | Description                                                                                                      |
|:------------|:-------|:---------|:-----------------------------------------------------------------------------------------------------------------|
| is_country  | int    | yes*     | Retrieve a list of countries (value 1)                                                                           |
| is_canton   | int    | yes*       | Retrieve a list of cantons (value 1)                                                                             |
| is_district | int    | yes*       | Retrieve a list of districts (value 1)                                                                           |
| is_zone     | int    | yes*       | Retrieve a list of zones (value 1)                                                                               |
| is_quarter  | int    | yes*       | Retrieve a list of quarter (value 1)                                                                             |
| country_id  | int    | no       | ID of a country to filter on                                                                 |
| canton_id  | int    | no       | ID of a canton to filter on                                                                 |
| district_id  | int    | no       | ID of a district to filter on                                                                 |
| zone_id  | int    | no       | ID of a zone to filter on                                                                 |
| quarter_id  | int    | no       | ID of a quarter to filter on                                                                 |
| lang        | string | yes      | Content languages in lower case (fr, en, it, de). Multiple languages can be retrieved using the "pipe" separator |

`* At least one of these attributes must be set`


## Response
application/json

#### Sample

```
{
    "199": {
        "country_id": "210",
        "canton_id": "22",
        "district_id": "6",
        "zone_id": "10",
        "labels": {
            "fr": "Lausanne",
            "en": "Lausanne",
            "de": "Lausanne"
        }
    },
    "370": {
        "country_id": "210",
        "canton_id": "25",
        "district_id": "1",
        "zone_id": "3",
        "labels": {
            "fr": "Anières",
            "en": "Anières",
            "de": "Anières"
        }
    },
    "385": {
        "country_id": "210",
        "canton_id": "25",
        "district_id": "1",
        "zone_id": "3",
        "labels": {
            "fr": "Cologny",
            "en": "Cologny",
            "de": "Cologny"
        }
    },
    ...
}
```
