# Brochures - Download
- This service is disabled by default for all websites. If you get an error, please call the support to see how to enable the brochures download process for a specific website.
- Before asking for the service to be enabled, be sure to respect the following rules : a brochure must not be downloaded more than 2 times a day, and a brochure must not be downloaded if the property or the development was not updated since the last synchronisation.
- This service sends to the client a PDF file containing the brochure file of a property or a development.


## Endpoint
```
POST https://brochures.realforce.ch/api/v1/download?lang={lang}&property_id={property_id}&promotion_id={promotion_id}&type={type}&color={color}&quality={quality}
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Body

| Name         | Type   | Required | Description                                                                                                      |
|:-------------|:-------|:---------|:-----------------------------------------------------------------------------------------------------------------|
| type         | string | yes      | Type of the brochure to send: brochure/prestige/2sides                                                           |
| color        | string | yes      | Color of the brochure to send: anonymous/standard                                                                |
| quality      | string | yes      | Quality of the brochure to send: email/print                                                                     |
| lang         | string | yes | Content languages in lower case (fr, en, it, de). Multiple languages can be retrieved using the "pipe" separator |
| property_id  | string    | yes*     | Property ID                                                                                                      |
| promotion_id | string    | yes*     | Promotion ID                                                                                                     |

`* These attributes are mutually exclusive`


## Response
application/pdf
