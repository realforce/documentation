# Promotions - List
Fetch a list of promotions accessible to the private API key.

## Endpoint
```
GET https://agency.realforce.ch/api/promotions/listall
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
     "uuid": "e9267fa7-3d09-11e6-982e-0050560100a5fe5dbbcea5ce7e2988b8c69bcfdfde8904aabc1f",
     "name": "LeS LuCiOleS",
     "reference": "LC-102",
     "city": "Lausanne",
     "status": "Actual",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug",
       "listings": [
         {
           "uuid": "5565733b57c8c-95f06351d86675d34b84f43e9542e455bd865573b8d329b6ee985c4f8cc59629",
           "reference": "PROPERTY1",
           "status": "Active"
         },
         {
           "uuid": "5565733b58196-544ed3fbd219677bcddc659e97ceea989de1d88a67adf4385b83f6a96ff85778",
           "reference": "PROPERTY2",
           "status": "Sold"
         }
       ]
     }
   },
   {
     "uuid": "58fe0bdb8f429-ab4dabe4411729bb6712386145b2c42519de9011006ce91095eb398fd499f136",
     "name": "Tremplin Bera",
     "reference": "NA-001PM",
     "city": "",
     "status": "Actual",
     "agency": {
       "id": "15",
       "name": "RF Test",
       "reference": "RO-3x0m50rd",
       "city": "Zug",
       "listings": [
         {
           "uuid": "5565733b57c8c-95f06351d86675d34b84f43e9542e455bd865573b8d329b6ee985c4f8cc59629",
           "reference": "PROPERTY3",
           "status": "Active"
         },
         {
           "uuid": "5565733b58196-544ed3fbd219677bcddc659e97ceea989de1d88a67adf4385b83f6a96ff85778",
           "reference": "PROPERTY4",
           "status": "Reserved"
         }
       ]
     }
   }
 ]
}
```
