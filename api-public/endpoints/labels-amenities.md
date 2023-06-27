# Labels - Amenities
Fetch "amenities" labels linked to the public data you retrieve from the public API endpoints.

## Endpoint
```
GET https://labels.realforce.ch/api/v1/get-amenities-labels?lang={lang}
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
        "fr": "Aire de jeu"
    },
    "2": {
        "fr": "Arrêt de bus"
    },
    "3": {
        "fr": "Banque"
    },
    "4": {
        "fr": "Centre sportif"
    },
    "5": {
        "fr": "Centre ville"
    },
    "6": {
        "fr": "Cinéma"
    },
    "7": {
        "fr": "Commerces"
    },
    "8": {
        "fr": "Crèche/Garderie"
    },
    ...
}
```
