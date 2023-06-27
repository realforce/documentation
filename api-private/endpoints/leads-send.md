# Leads - Send
Send a lead related to a property or a promotion for any portal or website accessible to the API key.

## Endpoint
```
POST https://agency.realforce.ch/api/leads/create
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Body

| Name                           | Type   | Required | Description                               |
|:-------------------------------|:-------|:---------|:------------------------------------------|
| date                           | date   | yes      | Lead date                                 |
| agency_id                      | int    | yes      | Agency ID                                 |
| message                        | string | yes      | Lead text content                         |
| gateway.type                   | string | yes      | Gateway type: website/portal              |
| gateway.id                     | string | yes      | Gateway ID                                |
| object.type                    | string | yes      | Object type: general/property/development |
| requester.title                | string | no       | Contact title: mr/ms                      |
| requester.lastname             | string | yes      | Contact lastname                          |
| requester.firstname            | string | no       | Contact firstname                         |
| requester.address.street_line1 | string | no       | Contact address street line 1             |
| requester.address.street_line2 | string | no       | Contact address street line 2             |
| requester.address.street_line3 | string | no       | Contact address street line 3             |
| requester.address.npa          | string | no       | Contact NPA (zip code)                    |
| requester.address.city         | string | no       | Contact city name                         |
| requester.address.country      | string | no       | Contact country as Alpha-2 ISO            |
| requester.phones.landline      | string | no       | Contact landline number                   |
| requester.phones.mobile        | string | no       | Contact mobile number                     |
| requester.email                | string | no       | Contact email                     |
| object.reference               | string | no*      | Object reference                          |
| object.id                      | string | no*      | Object ID                                 |
`* These attributes are mutually exclusive`

#### Sample

```
{
 "date": "2019-03-25T18:15:00+00:00",
 "agency_id": 123,
 "gateway": {
   "type": "website",
   "id": "436"
 },
 "object": {
   "type": "property",
   "id": "23789",
   "reference": "H-190235",
   "url": "https://www.myagency.ch/property/23789/details"
 },
 "requester": {
   "title": "mr",
   "lastname": "Davids",
   "firstname": "Mark",
   "address": {
     "street_line1": "avenue de Malagnou 54",
     "street_line2": "",
     "street_line3": "",
     "npa": "1208",
     "city": "Geneva",
     "country": "CH"
   },
   "phones": {
     "landline": "+41 22 123 45 67",
     "mobile": "+41 78 456 78 90"
   },
   "email": "mark.davids@gmail.com"
 },
 "message": "Dear sir, I would like to receive the documentation for this property. Thanks"
}
```


## Response
The HTTP response code will determine the request success or failure. In all cases, a string will be returned to explain the result.


#### Sample

```
{
 "message": "Lead created successfully"
}
```
