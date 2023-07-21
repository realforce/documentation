# Promotions - Details
Fetch published promotion' detailed public data.

## Endpoint
```
GET https://promotions.realforce.ch/api/v1/promotion/{promotion_id}
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Parameters

| Name          | Type   | Required                                                          | Description                                          |
|:--------------|:-------|:---------|:-----------------------------------------------------|
| promotion_id | string | yes | Promotion ID found in the promotion-summary endpoint |


## Response
application/json

#### Sample

```
{
    "id": "58feebd02e148-2e18b866f8d2c51ab9290f7707b0b685d216cb9055b4b3fefec7fb994b9e8966",
    "name": "Immo_Pulmann",
    "reference": "IM_NA_011",
    "logo": "",
    "location": "Berne",
    "country_id": 210,
    "canton_id": 2,
    "district_id": 30,
    "zone_id": 34,
    "city_id": 667,
    "quarter_id": 678,
    "environment_id": null,
    "apt_available": 14,
    "apt_sold": 4,
    "apt_rented": 2,
    "apt_active": 6,
    "apt_reserved": 2,
    "price": 2500000,
    "currency": "CHF",
    "min_surface": 360,
    "max_surface": 360,
    "min_rooms": 4,
    "max_rooms": 5,
    "min_bedrooms": 2,
    "max_bedrooms": 3,
    "longitude": null,
    "latitude": null,
    "map_zoom": null,
    "description": {
        "de": {
            "promotion_description": "",
            "location_description": "",
            "price_comment": "",
            "planning_comment": "",
            "extra_comment": "",
            "seo_title": null,
            "seo_keywords": null,
            "seo_description": null
        },
        "en": {
            "promotion_description": "",
            "location_description": "",
            "price_comment": "",
            "planning_comment": "",
            "extra_comment": "",
            "seo_title": null,
            "seo_keywords": null,
            "seo_description": null
        },
        "fr": {
            "promotion_description": "<p>Très belle appartement située au centre de la ville, facile d'accès et garage assuré.</p><p>Immeuble composé de 24 appartements, chacun dispose de 04 pièces dont 02 chambres.</p>",
            "location_description": "",
            "price_comment": "",
            "planning_comment": "",
            "extra_comment": "",
            "seo_title": null,
            "seo_keywords": null,
            "seo_description": null
        },
        "it": {
            "promotion_description": "",
            "location_description": "",
            "price_comment": "",
            "planning_comment": "",
            "extra_comment": "",
            "seo_title": null,
            "seo_keywords": null,
            "seo_description": null
        }
    },
    "photos": [
        {
            "url": "https://images.realforce.ch/static/images/websites/1a8f98728d1d984d190478686baa640156176ac9f721a4a12fc0fe39af7a86cd4fafa1505c66f6dbd632aea235900730eb11e6a0edfecf05bf714b01c97a386a.jpg",
            "title": null,
            "is_plan": false
        },
        {
            "url": "https://images.realforce.ch/static/images/websites/51bc5e51a95e93084aa754c1a9b0353c24d226e5a4598b8b25e91f457cae451ef09bae699d84de6c060ba01e4c54d326b5f8129ca75a48021a575cf32bd128ed.jpg",
            "title": null,
            "is_plan": false
        },
        {
            "url": "https://images.realforce.ch/static/images/websites/86a709292dbdefaa62e0acfac13800f7d26ef865b08ab616fe157991ad92f0a48d0a657ae4d7bcb53269d3b137809569d4b4af6836cb3a465c54a208f916235a.jpg",
            "title": null,
            "is_plan": false
        }
    ],
    "videos": [],
    "properties": [
            {
            "id": "5b14349bebc66-b02faaa2e8ff92540beb4e6b22d0915edd87599eb66ff907f7512a9af7098531",
            "status_id": 13,
            "status": "Sold",
            "position_id": 365,
            "position": "Floor",
            "reference": "A18026-11",
            "rooms": null,
            "floor": 1,
            "building_id": null,
            "building_name": null,
            "dimensions_habitable": 100.5,
            "dimensions_land": null,
            "dimensions_garden": null,
            "dimensions_balcony": 25.5,
            "dimensions_weighted": 113.25,
            "dimensions_floor": null,
            "dimensions_ground": null,
            "dimensions_ceiling": 2.9,
            "dimensions_terrace": null,
            "dimensions_acres": null,
            "dimensions_usable": null,
            "dimensions_garage": null,
            "dimensions_volume": null,
            "dimensions_basement": null,
            "dimensions_english_garden": null,
            "dimensions_lower_ground_floor": null,
            "dimensions_attic_floor": null,
            "dimensions_roofing_shelter": null,
            "dimensions_roof_top_terrace": null,
            "dimensions_veranda": null,
            "dimensions_ppe": null,
            "habitable": 100.5,
            "basement": null,
            "balcony": 25.5,
            "terrace": null,
            "garden": null,
            "weighted": 113.25,
            "price_on_request": true,
            "price": null,
            "raw_price": null,
            "price_weighted": null
        },
        {
            "id": "5b14349c0a9c0-841bd69fac6713a7516a30cea391fe5a5ff60e943a027c858a4ddcaca37c35e1",
            "status_id": 13,
            "status": "Sold",
            "position_id": 365,
            "position": "Floor",
            "reference": "A18026-14",
            "rooms": null,
            "floor": 1,
            "building_id": null,
            "building_name": null,
            "dimensions_habitable": 100.5,
            "dimensions_land": null,
            "dimensions_garden": null,
            "dimensions_balcony": 25.5,
            "dimensions_weighted": 113.25,
            "dimensions_floor": null,
            "dimensions_ground": null,
            "dimensions_ceiling": 2.9,
            "dimensions_terrace": null,
            "dimensions_acres": null,
            "dimensions_usable": null,
            "dimensions_garage": null,
            "dimensions_volume": null,
            "dimensions_basement": null,
            "dimensions_english_garden": null,
            "dimensions_lower_ground_floor": null,
            "dimensions_attic_floor": null,
            "dimensions_roofing_shelter": null,
            "dimensions_roof_top_terrace": null,
            "dimensions_veranda": null,
            "dimensions_ppe": null,
            "habitable": 100.5,
            "basement": null,
            "balcony": 25.5,
            "terrace": null,
            "garden": null,
            "weighted": 113.25,
            "price_on_request": true,
            "price": null,
            "raw_price": null,
            "price_weighted": null
        }
    ],
    "construction_plan": null,
    "payment_plan": [
        {
            "stage": "",
            "value": ""
        },
        {
            "stage": "",
            "value": ""
        }
    ],
    "contacts": [
        {
            "type": "Developer",
            "type_id": 25,
            "firstname": "Martin",
            "lastname": "Lecompte",
            "line1": null,
            "city": null,
            "zip": null,
            "phones": null,
            "email": "Mertin.le@yahoo.fr",
            "photo": ""
        }
    ]
}
```
