# Agencies - List
Fetch a list of agencies accessible to the private API key.

## Endpoint
```
GET https://agency.realforce.ch/api/agencies/listall
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
 "count": 1,
 "data": [
   {
     "id": "15",
     "name": "RF Test",
     "reference": "123456", // External ID to be used as partner_id in other endpoints
     "city": "Zug"
   }
 ]
}
```
