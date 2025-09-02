# Properties - List
Fetch a list of properties accessible to the private API key.

## Endpoint
```
GET https://agency.realforce.ch/api/properties/listall
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
 "count": 3,
 "data": [
   {
     "uuid": "56b9c6f1a32a2-52ed5973db954ec6db8836a42c81c5b47b2f2e13cecf719b0d6e2933a5a6869d",
     "reference": "TEST",
     "city": "Geneva",
     "status": "In process",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug"
     }
   },
   {
     "uuid": "56fe99df78235-0b3423c92b54a9e1bc445913acb64c4bdf33b16034fea7dfd17f2c8c1a02cc0c",
     "reference": "Erich",
     "city": "Safenwil",
     "status": "Active",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug"
     }
   },
   {
     "uuid": "56fe99dfed831-07cd19588e591b53b1fcad6456834ff8d4a941cdff0eb02142c581cfdc0d85b8",
     "reference": "Marc Sommer",
     "city": "Safenwil",
     "status": "Active",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug"
     }
   }
}
```
