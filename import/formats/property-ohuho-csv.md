# Property - Ohuho CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ID in your system |
| 15 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property reference |
| 6 | string | [Property Transaction Type](../values/property_transaction_type_id.md) | Property transaction type |
| 4 | string | [Property Category](../values/property_category_id.md) | Property category |
| 5 |  | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 9,18,19,23 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Property real location |
| 9,18,19,23 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Property alternate location |
| 31 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price |
| 11 | string | [Currency](../values/currency_id.md) | Property currency |
| 65 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of rooms |
| 51 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property habitable area |
| 85 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 28 | date | d.m.Y | d-m-Y | Y-m-d | Property mandate start date |
| 29 | date | d.m.Y | d-m-Y | Y-m-d | Property mandate end date |
| 13 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property floor |
| 160 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property title |
| 161 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property description |
| 54 | json | { "filename": string, "brochure_page"?: 0|0.5|1, "is_website"?: boolean, "is_portal"?: boolean, "is_plan"?: boolean } | Semicolon separated list of photos |
| 2 |  |  | owner ID |
| 32 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price per SQM |
| 58 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land area |
| 64 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property volume |
| 46 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year build |
| 47 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year renovated |
| 47 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property usable area |
| 21 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property visit3d |
| 83 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property monthly charges |
| 81 | json | { "filename": string, "is_brochure"?: boolean, "is_plan"?: boolean } | Semicolon separated list of documents |
| 48 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of floors |
| 27 | string | [Property Availability](../values/property_availability_id.md) | Property availability |
| 27 | date | d.m.Y | d-m-Y | Y-m-d | Property availability date |
| 99 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property monthly charges PPE |
| 201 | string | [Property Hotwater Type](../values/property_hotwater_type_id.md) | Property hotwater type |
| 200 | string | [Property Energy Type](../values/property_energy_type_id.md) | Property energy type |
| 202 | string | [Property State](../values/property_state_id.md) | Property state type |
| 48 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property ppe |
| 53 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property weighted |
| 74 | string | [Property Sell Foreigner](../values/property_sell_foreigner_id.md) | Property is allowed to foreigners |
| 68,69 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property sell price |
| 69,70,71 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property global commission |
| 69,70,71 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property global commission ercent |
| 39 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property annual charges |
| 38 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property parking price |
| 70 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | property notes seller |
| 24 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | property notes broker |

## Sample

[property-ohuho.csv](../samples/property-ohuho.csv)
```
idObject,idPerson,Proprietaire,Categorie,Type,Type de deal,Situation,Condition,Localite,Prix unitaire,Monnaie,Type residence,Etage,Type propriete,Reference,Titre,Titre 2,Adresse,Adresse 2,Site web,Tour virtuel,Video,Altitude,Commentaire,Description,Description PDF,Disponibilite,Date debut mandat,Date expiration mandat,Prix a partir de,Prix,Prix m2,Prix desire,Prix de reserve,Prix nettoyage,Taxe adulte,Taxe enfant,Prix parking,Charges,Rendement brut,Type rendement brut,Rendement net,Type rendement net,Etat locatif,Fond renovation,Annee construction,Annee renovation,Nb total etages,No Etage,No appartement,Surface habitable brute,Surface propriete,Surface au sol,Surface brute plancher,Densite terrain,Ponderation,Surface vente,Surface terrasse,Surface jardin hiver,Surface veranda,Surface balcon,Surface jardin,Surface cave,Volume,Nb pieces,Vendu ?,Vendu par autre,Date vente,Prix vente,Commission,Type commission,TVA incluse,Commission partagee,Vente aux etrangers,Exclusivite,Vues,Telechargements,Impressions,Visites,Images,PDFs,Pieces,Attributs,Liste telechargements,idCourtier
11531,45986,Laurent Christmann,Maison,Chalet,Vente,Chalets,,1996 Saclentz (Nendaz),Prix à la vente,CHF,Secondaire,,,ALP-11531,Chalet 4.5 pièces Arbaï Laurent Christmann,Magnifique chalet en vieux bois,Arbaï,,,,,,Route de Saclent,Magnifique chalet dans le pet,Magnifique chalet dans le petit village d,,,,0,1290000.00,10320.00,0.00,1290000.00,0.00,0.00,0.00,,0.00,0.00,VALUE,0.00,VALUE,0.00,0.00,2012,,2,,,,756.00,,,,0.00,125.00,,,,,,,,4.50,0,0,,0.00,3.00,PERCENTAGE,0,0,1,0,4,8,,,https://www.ohuho.com/src/uploads/objects/11531/orig_Vente-Saclentz-Nendaz-Maison-Chalet-98110f9259debf60ddff41407ea72e3d-1.jpg,https://www.ohuho.com/src/uploads/objects/11531/PlanArbai.pdf|Plan Arbaï|https://www.ohuho.com/src/uploads/objects/11531/Extraitdecadastre.pdf|Extrait de cadastre|https://www.ohuho.com/src/uploads/objects/11531/Declarationdescharges.pdf|Déclaration des charges|https://www.ohuho.com/src/uploads/objects/11531/Situation.pdf|Situation|https://www.ohuho.com/src/uploads/objects/11531/Parcelle.pdf|Parcelle|,Balcon | Loggia: 1Buanderie privée: 1Chambre double / parentale: 3Coin-repas: 1Cuisine: 1Jardin: 1Local technique: 1Réduit / Rangement: 1Salle de douche: 2Séjour: 1Terrasse: 1WC lavabo: 1Garage double: 1,"Environnement: Cadre verdoyant, Calme | Tranquille, Montagne, StationVue: Imprenable, Sur la vallée, Sur les montagnesExposition: Est, Nord, SudProximité: Banques, Centre sportif, Commerces, Crèche, Ecoles primaires, Loisirs, Pistes de ski, Poste, Remontées mécaniques, Restaurant, Transports publicsExtérieur: Aménagé, Arbustes, Jacuzzi, Terrasse couverteIntérieur: Boisé, Contemporain, Cuisine ouverte, Dressing, Grande surface vitrée, Lave linge, Lumineux, Sèche lingeEquipement primaire: Canalisations=Réseau communal, Eau=Réseau communal, Energie=Réseau électriqueEquipement technique: Buanderie équipée=Oui, Chauffage principal=Pompe à chaleur air-air, Internet=Oui, Mode de chauffage=Au sol, Porte du garage électrique=Oui, Télévision=Câble","2023-09-07 15:55:26, OTHER, Alp Real Estate SA - Sophie Gaidon2023-09-05 14:19:31, detailsClientHD, Alp Real Estate SA - Sophie Gaidon",CLEEDO1024
```
