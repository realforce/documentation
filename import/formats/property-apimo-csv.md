# Property - Apimo CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ID in your system |
| 2 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property reference |
| 3 | string | [Property Status](../values/property_status_id.md) | Property status |
| 3 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is archived |
| 4 | string | [Property Transaction Type](../values/property_transaction_type_id.md) | Property transaction type |
| 5 | string | [Property Category](../values/property_category_id.md) | Property category |
| 5 |  | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 7,8,10,11 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Property real location |
| 17 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property price |
| 19 | string | [Currency](../values/currency_id.md) | Property currency |
| 20 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of rooms |
| 21 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of bedrooms |
| 22 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property habitable area |
| 26 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 31 | string | [Property Mandate Type](../values/property_mandate_type_id.md) | Property transaction type |
| 33 | date | d.m.Y | d-m-Y | Y-m-d | Property mandate start date |
| 34 | date | d.m.Y | d-m-Y | Y-m-d | Property mandate end date |
| 35 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property floor |
| 41 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property title |
| 48 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property description |
| 54 | json | { "filename": string, "brochure_page"?: 0|0.5|1, "is_website"?: boolean, "is_portal"?: boolean, "is_plan"?: boolean } | Semicolon separated list of photos |
| 55 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Property creation date & time |
| 56 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Property update date & time |
| 57 |  |  | owner ID |

## Sample

[property-apimo.csv](../samples/property-apimo.csv)
```
Apinumber,Référence,Étape,Catégorie,Type,Pays,Adresse,Adresse,Résidence,Code postal,Ville,Quartier,Propriétaire,Téléphone,e-mail,Co-agent,Prix,Montant propriétaire,Monnaie,Pièces,Chambres,Surface,Lot,Numéro de clef,Agence,Utilisateur,Origine,Origine précise,Honoraire propriétaire,Honoraire acheteur,Mandat,Référence,Démarrage mandat,Fin mandat,Étage,Montant compromis,Vendu le,Groupe,Attributs,Titre En,Titre Fr,Titre De,Titre It,Titre Es,Titre Pt,Titre Ru,Commentaire En,Commentaire Fr,Commentaire De,Commentaire It,Commentaire Es,Commentaire Pt,Commentaire Ru,Photos,Créé le,Mise à jour le
6948096,6565,Retiré par l'agence,Vente,Terrain constructible,Suisse,En Praudi 23,,,1306,Daillens,,M. DUSALON,+41 79 287 09 09,,,,,CHF,,,,m²,,Immo Plus,Service DES VENTES123,,,0,0,,,,,,,,Prospection,,,,,,,,,,,,,,,,,2022-04-28 10:32:08,2022-04-28 11:26:19
```
