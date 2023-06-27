# Portals - List
Fetch a list of portals accessible to the private API key.

## Endpoint
```
GET https://agency.realforce.ch/api/portals/listall
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
 "count": 4,
 "data": [
   {
     "id": "56",
     "partner_id": null,
     "label": "Previsite",
     "portal_type": "Previsite",
     "portal_type_id": 9,
     "website_id": null,
     "reference": "p145e12",
     "active": true,
     "transfer_active": true,
     "language": "fr",
     "last_execution_date": "2019-10-22T20:00:01+02:00",
     "last_status": "ok",
     "last_status_message": "Transfert done of 0 properties with success...",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug"
     }
   },
   {
     "id": "74",
     "partner_id": null,
     "label": "Immoscout 24",
     "portal_type": "Immoscout 24",
     "portal_type_id": 3,
     "website_id": null,
     "reference": "12578549",
     "active": false,
     "transfer_active": false,
     "language": "fr",
     "last_execution_date": "2019-11-01T11:17:38+01:00",
     "last_status": "error",
     "last_status_message": "",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug"
     }
   },
   {
     "id": "75",
     "partner_id": null,
     "label": "Luxury Estate Test",
     "portal_type": "Luxury Estate",
     "portal_type_id": 11,
     "website_id": null,
     "reference": "a12hn4587h",
     "active": false,
     "transfer_active": true,
     "language": "fr",
     "last_execution_date": "2017-08-22T16:50:27+02:00",
     "last_status": "ok",
     "last_status_message": "Transfert done of 7 properties with success...",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug"
     }
   },
   {
     "id": "107",
     "partner_id": null,
     "label": "Spiti360",
     "portal_type": "Spiti360",
     "portal_type_id": 18,
     "website_id": null,
     "reference": "1154",
     "active": true,
     "transfer_active": false,
     "language": "fr",
     "last_execution_date": "2019-02-22T10:00:02+01:00",
     "last_status": "error",
     "last_status_message": "Error on login to FTP server...",
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
