# Labels - Amenities categories
Fetch "amenities categories" labels linked to the public data you retrieve from the public API endpoints.

## Endpoint
```
GET https://labels.realforce.ch/api/v1/get-amenities-categories-labels?lang={lang}
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Parameters

| Name        | Type   | Required | Description                                                                                                      |
|:------------|:-------|:---------|:-----------------------------------------------------------------------------------------------------------------|
| lang        | string | yes      | Content languages in lower case (fr, en, it, de). Multiple languages can be retrieved using the "pipe" separator |


## Response
application/json

#### Sample

```
{
    "1": {
        "fr": "Entourage"
    },
    "2": {
        "fr": "Extérieur"
    },
    "3": {
        "fr": "Intérieur"
    },
    "4": {
        "fr": "Equipement"
    },
    "5": {
        "fr": "Revêtements intérieur"
    },
    "6": {
        "fr": "Revêtements extérieur"
    },
    "7": {
        "fr": "Revêtements des toits"
    },
    ...
}
```
