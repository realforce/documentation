# Promotions - List
Fetch a list of published promotions' summary public data.

## Endpoint
```
GET https://promotions.realforce.ch/api/v1/promotions?per_page={per_page}&page={page}&lang={lang}
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Parameters

| Name     | Type   | Required                                                          | Description                                                                                                      |
|:---------|:-------|:------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------|
| per_page | int    | yes                                                               | Number of records to retrieve per page (max 100)                                                                          |
| page     | int    | yes | Index of the page to retrieve                                                                                    |
| lang     | string | yes | Content languages in lower case (fr, en, it, de). Multiple languages can be retrieved using the "pipe" separator |


## Response
application/json

#### Sample

```
{
    "count": 2,
    "page": 1,
    "per_page": 20,
    "data": [
        {
            "id": "e9267fa7-3d09-11e6-982e-0050560100a5fe5dbbcea5ce7e2988b8c69bcfdfde8904aabc1f",
            "name": "Les Lucioles",
            "logo": "",
            "reference": "LC-102",
            "location": "Lausanne",
            "description": "",
            "apt_available": 15,
            "apt_active": 1,
            "apt_reserved": 1,
            "price": 2500,
            "currency": "CHF",
            "min_surface": 125,
            "max_surface": 1500,
            "min_rooms": 4,
            "max_rooms": 24,
            "min_bedrooms": 5,
            "max_bedrooms": 6,
            "photos": [
                {
                    "url": "https://images.realforce.ch/static/images/websites/60ead4640af5d0b48a7b949d1e1896d6d57fc1564805c58ea3adacda3294b0d5792baa7a14cf3a694b60af776b05a9c5612a9619c37c0ec380a5360e44eed530.jpg",
                    "title": null,
                    "is_plan": false
                },
                {
                    "url": "https://images.realforce.ch/static/images/websites/f6f64252392e53264a7fa23520e27093ec265ba475bf1b07944c87097486313c3160f5b2db23a04e0fddc58c4040c0a46e562a1a420204d6078ffab0de0d6d6c.jpg",
                    "title": null,
                    "is_plan": false
                },
                {
                    "url": "https://images.realforce.ch/static/images/websites/0d590ade4deaea418f398e4fe62c56d9d9af7499ad2d3f274fd7dda1698c757ee6c5f850e478dfab2ef11ecfb3bd622b0eabb080c139e7cd45b44ab7e1bffb49.jpg",
                    "title": null,
                    "is_plan": false
                }
            ],
            "property_ids": [
                "56729a28bf0dc-247c4509623ae6ab885903fd8699fe0c3faea0d3f0bcef6c1a95589cb4572150",
                "575eb700623dc-67cec7800db9ff7c8f401a86296427eb28c76b3fb8af8e996cab86d31562a5d8",
                "575eb70b231c0-53de0168ea3d2bb81a30acf53cec47e2704e30db3103bb75d11750c69ce03d9f"
            ]
        },
        ....
    ]
}
```
