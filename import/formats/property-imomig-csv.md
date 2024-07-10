# Property - Imomig CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ID in your system |
| 4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property reference |
| 14 | string | [Property Status](../values/property_status_id.md) | Property status |
| 14 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is archived |
| 12 | string | [Property Transaction Type](../values/property_transaction_type_id.md) | Property transaction type |
| 3 | string | [Property Category](../values/property_category_id.md) | Property category |
| 3 |  | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 22,23,24 | json | { "location_level": country|canton|district|zone|city|quarter, "location_name": string, "zip": string, "line1": string, "line2": string, "line3": string, "environment_id": string, "altitude": string, "longitude": string, "latitude": string } | Property real location |
| 85 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price |
| 19 | string | [Currency](../values/currency_id.md) | Property currency |
| 29 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of rooms |
| 33 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of bedrooms |
| 45 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property habitable area |
| 11 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 18 | string | [Property Mandate Type](../values/property_mandate_type_id.md) | Property transaction type |
| 19 | date | d.m.Y | d-m-Y | Y-m-d | Property mandate start date |
| 20 | date | d.m.Y | d-m-Y | Y-m-d | Property mandate end date |
| 32 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property floor |
| 160 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property title |
| 161 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property description |
| 161 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property location description |
| 54 | json | { "filename": string, "brochure_page"?: 0|0.5|1, "is_website"?: boolean, "is_portal"?: boolean, "is_plan"?: boolean } | Semicolon separated list of photos |
| 7 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Property creation date & time |
| 8 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Property update date & time |
| 204 |  |  | owner ID |
| 75 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price per SQM |
| 44 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land area |
| 66 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property volume |
| 73 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year build |
| 74 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Property year renovated |
| 115 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Property ceiling height |
| 47 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property usable area |
| 83 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property monthly charges |
| 28 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of bathrooms |
| 31 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property number of floors |
| 78 | string | [Property Availability](../values/property_availability_id.md) | Property availability |
| 79 | date | d.m.Y | d-m-Y | Y-m-d | Property availability date |
| 99 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property monthly charges PPE |
| 201 | string | [Property Hotwater Type](../values/property_hotwater_type_id.md) | Property hotwater type |
| 200 | string | [Property Energy Type](../values/property_energy_type_id.md) | Property energy type |
| 202 | string | [Property State](../values/property_state_id.md) | Property state type |
| 48 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property ppe |
| 53 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property weighted |
| 113 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | property lot |
| 131 | string | [Property Sell Foreigner](../values/property_sell_foreigner_id.md) | Property is allowed to foreigners |
| 43 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property dimensions approximative |
| 199 | string | [Property Heating Type](../values/property_heating_type_id.md) | Property heating type |
| 116 | date | d.m.Y | d-m-Y | Y-m-d | Property definitive sell update date |
| 117 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property sell price |
| 118 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property global commission |
| 132 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property commission for broker |

## Sample

[property-imomig.csv](../samples/property-imomig.csv)
```
ID de compte,Société,Catégorie,Référence immoMiG,Nom du projet,Référence parente,Insertion,Dernière modification,Partage,Facturation publication,Courtier responsable,Type,Réf. agence,Statut,Acquisition,Contact visite,Type,Exclusivité,Date de début de mandat,Date d'échéance,Date de la réservation,NPA,Lieu,Adresse,Adresse de remplacement,Pays,Nbr. WC,Nbr. salles d'eau,Nbr. pièces,Prix à la pièce/an,Nbr. étages,Etage,Nbr. chambres à coucher,Nbr. logements,Sous-sol,Nombre de dépôts,Nbr. commerces,Année rénovation,Equipé,Rendement net,Rendement brut,Parking possible,"""~"" devant les dimensions",Surface terrain,Surface habitable,Surface habitable totale,Surface utile,Surface PPE,Surface terrasse,Surface balcon,Surface veranda / jardin d'hiver,Surface loggia,Surface pondérée,Surface sol bâtiment,Surface brute de plancher,Surface nette,Surface sous-sol,Surface totale,Surface nette,Surface cave,Surface grenier,Surface locative,Surface bâtie,Surface non-bâtie,Surface dépôt,Volume,Impôt communal,Impôt paroissial,Impôt cantonal,Indice d'utilisation du sol,Coefficient d'occupation du sol,Impôt immobilier,Année construction,Année de rénovation,Prix/m²,Prix moyen/m²,Prix locaux commerciaux/an,Disponibilité,Date de disponibilité,Saison,Année,Charges,Montant charges,Prix/m²,Prix,Estimation,Prix ​​à partir de,Nombre de place de parc,Nombre de place de parc int.,Nombre de place de parc ext.,Nombre de box,Prix place(s) de parc,Prix places de parc int.,Prix places de parc ext.,Prix box,Prix sur demande,Loyer subventionné,Commentaires,Charges PPE,Montant fonds de rénovation,Etat fond de rénovation,Etat locatif brut,Etat locatif net,No RF,No assurance incendie,Altitude (m),Zone construction,Evacuation eaux usées,Cédules hypothécaires existantes,Densité,Charges d'exploitation,Valeur fiscale,Lot,Forme juridique,Hauteur plafond,Date de la transaction,Montant de la transaction,Montant de la commission,Vendeur/Utilisateur,Acheteur/Locataire,Comment l'acheteur a pris connaissance du bien,Date d'entrée en jouissance,Date de début du bail,Prix sans charges,Charges,No de facture,Garantie,Délai de paiement prévu,Date du paiement de la commission,Remarques transaction,Vente autorisée aux étrangers,Montant commission courtier responsable,Commission courtier,Taux de commission courtier intermédiaire,Taux de commission courtier responsable,Société,Type de contact,Titre,Prénom,Nom,Profession,Case postale,Adresse,Case postale,Code postal,Ville,Téléphone,Tél. prof.,Fax,Mobile,Tél. direct,E-mail,MLS proposé à,Etage,Période,Montant des coûts de l'annexe,Coûts de l'annexe par période,Latitude,Longitude,Titre,Descriptif / Tour d'horizon rapide,Descriptif pour passerelles,Premier coup d'oeil,Situation,Accès,Commerces,Transports,Loisirs,Construction,Sous-sol,Rez inférieur,Rez-de-chaussée,Rez supérieur,1er niveau,2ème niveau,3ème niveau,4ème niveau,Combles,Annexe(s),Aménagements extérieurs,Toiture,Particularités,Sous-titre,Remarques,Parcelle 1,Parcelle 2,Parcelle 3,Parcelle 4,Parcelle 5,Commune,Type de site web pour le projet,Images,Titres d'images,Descriptions d'images,Droit de superficie,Date d'échéance,Rente du droit de superficie,Période,Installation chauffage,Type de chauffage,Eau chaude sanitaire,Condition,Valeur assurance bâtiment
1100,Veyrat-Sarasin SA,Hôtel particulier,2478828,,,14.01.2020,14.01.2020,Non,Oui,VEYRAT S,À vendre,,En cours d'insertion,,-@@@-@@@-,,Non,,,,1206,Genève,Rue François 16,,Suisse,,,,,,,,,,,,,,,,Non,,,900.0,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,Immédiatement,,,,,,,30000000.00,,,,,,,,,,,Non,Non,Hotel particulier de 900m2  travaux prévu : toit et isolation  2 appartements de 200m2 liés l'un a l'autre à l'étage  Locaux commerciaux en travaux au rez ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,2,,,,,,Monsieur,,n,Tamp ,,,,,,,,,,796138389,,,,,Mois,,,46.198582,6.152711,Hotel particulier de charme - Vielle Ville @@@-@@@-@@@-,Hotel particulier de charme - Vielle Ville@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,-@@@-@@@-@@@-,https://1100.ch/fr/objects/detail/2478828,,,,Non,30.11.-0001,,An,,,,,
```
