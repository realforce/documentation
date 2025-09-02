# Properties - List
Fetch a list of published properties' public data.

## Endpoint
```
GET https://listings.realforce.ch/api/v1/get-full-listings?per_page={per_page}&page={page}&lang={lang}
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Parameters

| Name            | Type   | Required | Description                                                                                                      |
|:----------------|:-------|:---------|:-----------------------------------------------------------------------------------------------------------------|
| per_page        | int    | yes      | Number of records to retrieve per page (max 100)                                                                          |
| page            | int    | yes      | Index of the page to retrieve                                                                                    |
| lang            | string | yes      | Content languages in lower case (fr, en, it, de). Multiple languages can be retrieved using the "pipe" separator |
| update_date_min | date (format YYYY-MM-DD)       | no       | Filter only the properties after the date give in parameter |
| update_date_max | date (format YYYY-MM-DD)       | no       | Filter only the properties before the date give in parameter |


## Response
application/json

#### Sample

```
{
    "count": 5,
    "page": 1,
    "per_page": 100,
    "data": [
        {
            "id": "575eb70b231c0-53de0168ea3d2bb81a30acf53cec47e2704e30db3103bb75d11750c69ce03d9f",
            "creation": "2017-04-20 13:37:00",
            "lastupdate": "2017-04-21 16:00:59",
            "availability_id": "4",
            "source_id": "174",
            "mandate_type_id": null,
            "main_category_id": "2",
            "sub_category_id": "149",
            "reference": "AA1-5",
            "promotion_reference": null,
            "mandate_start": null,
            "mandate_end": null,
            "lot": "",
            "parcel": "",
            "building": "",
            "availability_date": null,
            "lease_type": null,
            "direct_transaction": "1",
            "transaction_type_id": "2",
            "status_id": "9",
            "ranking": "1",
            "off_plan": "1",
            "cadastre_number": "",
            "cadastre_zone": "",
            "sell_date": null,
            "prestige": null,
            "new_construction": "0",
            "sonority_id": null,
            "garage_id": "27",
            "hotwater_type_id": null,
            "heating_energy_type_id": null,
            "heating_type_id": null,
            "minergy_id": null,
            "furnish_id": null,
            "position_id": "114",
            "style_id": "85",
            "view_id": "76",
            "sunlight_id": null,
            "orientation_id": null,
            "state_id": null,
            "floor": "2",
            "top_floor": "0",
            "floors": null,
            "toilets": null,
            "bedrooms": "5",
            "bathrooms": "2",
            "showerrooms": null,
            "rooms": "4",
            "garage_capacity": null,
            "construction_year": null,
            "renovation_year": null,
            "face_to_face": "0",
            "environment_id": null,
            "country_id": "210",
            "quarter_id": "199",
            "city_id": "199",
            "zone_id": "10",
            "district_id": "6",
            "canton_id": "22",
            "longitude": "8.7351356",
            "latitude": "47.2392343",
            "map_zoom": "9",
            "currency_id": "49",
            "scheme_id": null,
            "charges_included_id": null,
            "individual_charges_included_id": null,
            "parking_included_id": null,
            "parking_mandatory_id": null,
            "maintenance_contract_included_id": null,
            "incidental_expenses": null,
            "frequency_id": null,
            "price": "1900000",
            "goodwill": null,
            "original": null,
            "parking": "1",
            "m2": "7465.61",
            "monthly_charges": null,
            "annual_charges": null,
            "monthly_charges_ppe": null,
            "monthly_charges_heating": null,
            "renovation_funds": null,
            "tax": "",
            "income": "",
            "billag": null,
            "sig": null,
            "deposit": null,
            "habitable": "165",
            "ppe": null,
            "land": "144",
            "garden": null,
            "balcony": "100",
            "weighted": "254.5",
            "m2_floor": null,
            "ground": null,
            "ceiling": null,
            "terrace": "13",
            "acres": null,
            "usable": "300",
            "garage": "150",
            "volume": null,
            "basement": "110",
            "zip": "8712",
            "address1": null,
            "address2": null,
            "address3": null,
            "website_featured": "0",
            "publication_date": "2020-12-28 10:40:59",
            "website_homepage": "0",
            "broker_id": "yv4dISLuCRTBRF9zCRNUyKF2YLChKw5-P0OPyN3CmpI=",
            "broker_lastname": "Charlie",
            "broker_firstname": "Do",
            "broker_email": "info@realforce.ch",
            "broker_phone": "+41 848 11 11 11",
            "broker_mobile": "+41 078 111 11 11",
            "publisher_id": "6541",
            "view_ids": [
                76,
                80,
                82
            ],
            "buyers": [
                "111": {
                    "contact_id": "111",
                    "firstname": "Alice",
                    "lastname": "Smith"
                },
                "112": {
                    "contact_id": "112",
                    "firstname": "Bob",
                    "lastname": "Smith"
                }
            ],
            "property_sell": {
                "last_deposit_date": "2019-08-04",
                "deposit_amount": "123456.00",
                "signature_date": "2019-08-05"
            },
            "photos": [
                "https://images.realforce.ch/static/images/websites/b5387f9d98fb8faf8c58dae740774fa7ffac1891fcc3e962fb7dd92c5b630be11bc5474b01e55d19294cb2fe882d3eddef554e48cc8815b23556bdd04473bb2c.jpg",
                "https://images.realforce.ch/static/images/websites/0b60c2d594c6b88f9b145b1c97ab0d38d7a66a31c1be39f2508ecd05ab99d8fa6a96f14be9462bf0415811232ff7997a98996c75f0705a495fe774fa02de5136.jpg",
                "https://images.realforce.ch/static/images/websites/75e145f22dc16c6885e747fad64df722da6a65a0fb4bf99c8d09faf877481d6b9984d2daabfbbcf7a5ed4711885825b9924bfe7d802a7b75c30162dbe26d5e5e.jpg",
                "https://images.realforce.ch/static/images/websites/eb66b98b42159156b4fa810cff78a570b7773f93a229c62945af2643aaae888bd4adf299ffe8f05623b4c007b6465d7a4e6552f1990c4a702caddaae6a70dfe5.jpg",
                "https://images.realforce.ch/static/images/websites/92f4995a9b5182a2a5704b3001dc2994a08970658c3470f0b2a7577404148196eb134c41e15ad9ad37cfde43ea2aec87d5bbf62ab23c220b73c486708ce5e451.jpg"
            ],
            "photosObject": [
                {
                    "url": "https://images.realforce.ch/static/images/websites/b5387f9d98fb8faf8c58dae740774fa7ffac1891fcc3e962fb7dd92c5b630be11bc5474b01e55d19294cb2fe882d3eddef554e48cc8815b23556bdd04473bb2c.jpg",
                    "isPlan": false,
                    "titles": {
                        "en": ""
                    }
                },
                {
                    "url": "https://images.realforce.ch/static/images/websites/0b60c2d594c6b88f9b145b1c97ab0d38d7a66a31c1be39f2508ecd05ab99d8fa6a96f14be9462bf0415811232ff7997a98996c75f0705a495fe774fa02de5136.jpg",
                    "isPlan": false,
                    "titles": {
                        "en": ""
                    }
                },
                {
                    "url": "https://images.realforce.ch/static/images/websites/75e145f22dc16c6885e747fad64df722da6a65a0fb4bf99c8d09faf877481d6b9984d2daabfbbcf7a5ed4711885825b9924bfe7d802a7b75c30162dbe26d5e5e.jpg",
                    "isPlan": false,
                    "titles": {
                        "en": ""
                    }
                }
            ],
            "amenities": [
                "56",
                "142",
                "57",
                "58",
                "59"
            ],
            "amenitiesObject": [
                {
                    "id": "56",
                    "value": null
                },
                {
                    "id": "142",
                    "value": null
                },
                {
                    "id": "57",
                    "value": null
                },
                {
                    "id": "58",
                    "value": null
                },
                {
                    "id": "59",
                    "value": null
                }
            ],
            "videosObject": [],
            "description": {
                "en": {
                    "title": "Wonderfull House",
                    "description": "The house is situated in a quiet location close to the beautiful Lake Zurich-shore. The bus stop is a 2-minute walk away. In 30-minute intervals, the bus will take you to the train station Zurich, from where the S7 leads within 24 minutes to Stadelhofen station. A footpath leads to the center of Stäfa. The public, unique and romantic lakeside \"Sunneshy\" with restaurant and bathing without supervision is located in close proximity.",
                    "summary_title": "",
                    "summary_description": "",
                    "seo_title": "",
                    "seo_keywords": "",
                    "seo_description": ""
                }
            },
            "broker_avatar": "https://images.realforce.ch/static/images/websites/d3e498a8bb6cb4157c30c29ec3d649c08762c04dd2d3299f30b56c2d4d220fb518e3fe3dd715920ba19f65278f0830529ea7d50ded1241b0bff0c7b5921c1495.png"
        },
        ...
    ]
}
```
