# Labels - Amenities groups
Fetch "amenities groups" to place each amenity within its amenity-category.

## Endpoint
```
GET https://labels.realforce.ch/api/v1/get-amenities-groups
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Parameters
This endpoint does not support any parameter.


## Response
application/json

#### Sample

```
{
    "1": [
        "1",
        "2",
        "3",
        "4",
        "5",
        "6",
        "7",
        "8",
        "9",
        "10",
    ],
    "2": [
        "29",
        "30",
        "31",
        "32",
    ],
    ...
}
```
