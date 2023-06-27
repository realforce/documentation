# Leads - Send
Send a lead related to a property or a promotion.

## Endpoint
```
POST https://leads.realforce.ch/api/v1/lead
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Body

| Name               | Type   | Required | Description                                                                                                     |
|:-------------------|:-------|:---------|:----------------------------------------------------------------------------------------------------------------|
| sender_message     | string | yes      | Message that the requester wants to send to the agency                                                          |
| date               | int    | yes      | Timestamp of the request (in seconds)                                                                           |
| sender_firstname   | string | no       | Requester's firstname                                                                                           |
| sender_lastname    | string | no       | Requester's lastname                                                                                            |
| sender_email       | string | no       | Requester's email                                                                                               |
| sender_number      | string | no       | Requester's phone number                                                                                        |
| property_reference | string | yes*     | Property reference                                                                                              |
| property_id        | string    | yes*     | Property ID                                                                                                     |
| promotion_id       | string    | yes*     | Promotion ID                                                                                                    |
`* These attributes are mutually exclusive`

#### Sample

```
{
    "sender_message" : "My message",
    "date" : "1458753987",
    "sender_firstname" : "Pascal",
    "sender_lastname" : "Dupond",
    "sender_mail" : "pascal@dupond.ch",
    "sender_number" : "+41 76 625 90 45",
    "property_id" : "575eb70b231c0-53de0168ea3d2bb81a30acf53cec47e2704e30db3103bb75d11750c69ce03d9f"
}
```


## Response
application/json

#### Sample

```
{
    "success": true,
    "id": "s87fdf54",
    "message": "Lead saved successfully."
}
```
