# Search - Apimo CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 38 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search ID in your system |
| 1 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Contact ID this search is linked to |
| 7 | string | [Search Transaction Type](../values/search_transaction_type_id.md) | Property transaction type |
| 8 | string | [Property Category](../values/property_category_id.md) | Property category |
| 8 |  | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 9 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price min |
| 10 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price max |
| 12 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room min |
| 12 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room max |
| 12 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property bedroom min |
| 8,13 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property area min |
| 14 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property area max |
| 8,13 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land min |
| 8,14 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land max |
| 16,17 | json | { "level": country|canton|district|zone|city|quarter, "name": string } | Search locations |
| 18 | date | d.m.Y | d-m-Y | Y-m-d | Search update date |
| 19,39 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search private comment |
| 22 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |

## Sample

[search-apimo.csv](../samples/search-apimo.csv)
```
Contact Référence,Contact,Classification,Téléphone,e-mail,Co-agence,Catégorie,Type,Prix min,Prix max,Monnaie,Pièces,Surface min,Surface max,Lot,Ville,Quartier,Action,Commentaire,,Date,Utilisateur,Mailing,e-mailing,Magazine,Origine,Origine précise,Langue parlée 1,Langue parlée 2,Date de naissance,Lieu de naissance,Adresse,Adresse,Code postal,Ville,Pays,Agence,Référence,Critères complémentaires,Attributs
8751280,Aco PECTORO,,+41 79 370 90 08,aco.pectoro@bluewin.ch,,Vente,Appartement,665 000,1 235 000,CHF,≥ 3.0 chambres,,,Mètre carré,Lausanne,GRAND LAUSANNE,08/12/22,"""""",,24/05/18,Service DES VENTES123,Non abonné,Non abonné,Non abonné,,,français,,,,,,,,Suisse,Immo Plus,2496309,"""""",
```
