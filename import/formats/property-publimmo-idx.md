# Property - Publimmo IDX

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 6,7,8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ID in your system |
| 6,7,8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property reference |
| 3 | string | [Property Category](../values/property_category_id.md) | Property category |
| 3,4 |  | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 5,19,20 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price |
| 21 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property monthly charges |
| 23 | string | [Currency](../values/currency_id.md) | Property currency |
| 80 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 28 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property habitable area |
| 29 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land area |
| 30 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property usable area |
| 26 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of rooms |
| 16 | string | [Property Availability](../values/property_availability_id.md) | Property availability |
| 5 | string | [Property Transaction Type](../values/property_transaction_type_id.md) | Property transaction type |
| 16 | date | d.m.Y | d-m-Y | Y-m-d | Property availability date |
| 9,10,11 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Property real location |
| 9,10,11 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Property alternate location |
| 65 | json | { "filename": string, "is_brochure"?: boolean, "is_plan"?: boolean } | Semicolon separated list of documents |
| 47,48,49,50,51,88,89,90,91,143,144,145,146 | json | { "filename": string, "brochure_page"?: 0|0.5|1, "is_website"?: boolean, "is_portal"?: boolean, "is_plan"?: boolean } | Semicolon separated list of photos |
| 25 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property floor |
| 31 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property volume |
| 34,35,36,37,38,39,40,41,42,43,45,109,116,117,120,123,169,175 | json | { "amenity_id": string, "amenity_value": string } | amenities |
| 17 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property title |
| 18 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property description |
| 32 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year build |
| 110 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ceiling height |
| 163 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of floors |
| 164 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year renovated |
| 171 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is new |
| 181 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property visit3d |

## Sample

[property-publimmo.idx](../samples/property-publimmo.idx)
```
IDX3.01#Publimmo v1#HOUSE#5#SALE###826588##1261#Le Vaud#VD#CH####Maison 4.5 pièces à Le Vaud#Le Mont-Blanc dans votre salon...<br><br>Cette charmante villa familiale de 4,5 pièces (+ sous-sol) offre confort et luminosité dans un cadre idyllique de verdure avec une vue dégagée sur le Mont-Blanc depuis la pièce à vivre.<br><br>Située dans un quartier paisible à quelques pas du Zoo de la Garenne, la propriété permet d'accéder à pieds au centre du village ou vous trouverez tout le nécessaire (école, crèche, épicerie, restaurant, bus, etc.).#1290000###SELL#CHF###4.5##100#1450#156#815#######Y#Y########8428753.jpg#8428754.jpg#8428755.jpg####Terrasse avec vue sur le Mont-Blanc#Salon (avec vue sur le Mont-Blanc également)###############test#CFP Immo Conseils###Chemin du Crêt 13B#1261#Le Vaud#CH#022 366 75 27 ###test.idxv3@test.net###############################################http://www.acheter-louer.ch/fr/achat-immobilier/cfpimmoconseils/le%c2%a0vaud.html###################################################01.12.2022 14:42:27###https://my.matterport.com/show/?m=8jEz4r##
```
