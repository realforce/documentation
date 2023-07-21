# Labels - Categories
Fetch "categories" labels linked to the public data you retrieve from the public API endpoints.

## Endpoint
```
GET https://labels.realforce.ch/api/v1/get-categories-labels?lang={lang}
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
        "fr": "Appartement"
    },
    "2": {
        "fr": "Maison"
    },
    "100": {
        "fr": "Appartement"
    },
    "102": {
        "fr": "Duplex"
    },
    ...
}
```
