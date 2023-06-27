# Labels - Choices
Fetch "choices" labels linked to the public data you retrieve from the public API endpoints.

## Endpoint
```
GET https://labels.realforce.ch/api/v1/get-choices-labels?lang={lang}&category={category}
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Parameters

| Name     | Type   | Required | Description                                                                                                      |
|:---------|:-------|:---------|:-----------------------------------------------------------------------------------------------------------------|
| category | int    | yes      | Choice category ID                                                                                               |
| lang     | string | yes      | Content languages in lower case (fr, en, it, de). Multiple languages can be retrieved using the "pipe" separator |


## Response
application/json

#### Sample

```
{
    "1": {
        "fr": "Location"
    },
    "2": {
        "fr": "Vente"
    },
    ...
}
```
