# Websites - List
Fetch a list of websites accessible to the private API key.

## Endpoint
```
GET https://agency.realforce.ch/api/websites/listall
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
 "count": 2,
 "data": [
   {
     "id": "31",
     "partner_id": null,
     "url": "www.demo-barcelona.realforce.ch",
     "alternate_urls": [
       "demo-barcelona.realforce.ch"
     ],
     "languages": [
       "de",
       "en",
       "fr"
     ],
     "layout": "full",
     "template": "template_3",
     "active": true,
     "fisher": false,
     "private_api_key": "<api_key>",
     "public_api_key": "<api_key>",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug"
     }
   },
   {
     "id": "48",
     "partner_id": null,
     "url": "www.realforce.ch",
     "alternate_urls": [
       "www.realforce.ch",
       "demo-geneva.realforce.ch"
     ],
     "languages": [
       "de",
       "en",
       "fr"
     ],
     "layout": "full",
     "template": "template_4",
     "active": true,
     "fisher": true,
     "private_api_key": "<api_key>",
     "public_api_key": "<api_key>",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug"
     }
   }
 ]
}
```
