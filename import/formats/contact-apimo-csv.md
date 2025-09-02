# Contact - Apimo CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact ID in your system |
| 3 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 5 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact company name |
| 6,18 | string | [Contact Title](../values/contact_title_id.md) | Contact title |
| 7,19 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact lastname |
| 8,20 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact firstname |
| 10,22,41 | json | { "notes": string, "value": string, "is_use_mailing": boolean, "is_main": boolean } | Semicolon separated list of emails |
| 11,12,23 | json | { "notes": string, "number": string, "type": mobile/landline, "is_main": boolean } | Semicolon separated list of phones |
| 14 | date | d.m.Y | d-m-Y | Y-m-d | Contact birthdate |
| 16,26,32 | string | [Country](../values/country_id.md) | Contact nationality |
| 28,29,30,31,32 | json | { "notes": string, "country_id": string, "line1": string, "line2": string, "line3": string, "city": string, "zip": string, "use_default": boolean } | Semicolon separated list of addresses |
| 33,35,37,38,42 | string | [Contact Type](../values/contact_type_id.md) | Semicolon separated list of contact types |
| 44,45 | string | [Language](../values/language_id.md) | Contact language |
| 53 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Contact creation date & time |
| 54 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Contact update date & time |
| 55 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact private comment |
| 24 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the sale broker in charge |
| 34,36 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is archived |

## Sample

[contact-apimo.csv](../samples/contact-apimo.csv)
```
Référence,Agence,Utilisateur,Type,Nom,Civilité,Nom de famille,Prénom,Profession,e-mail,Téléphone,Mobile,Télécopie,Date de naissance,Lieu de naissance,Nationalité,Numéro fiscal,Civilité,Nom de famille,Prénom,Profession,e-mail,Mobile,Date de naissance,Lieu de naissance,Nationalité,Numéro fiscal,Adresse,Adresse,Code postal,Ville,Pays,Propriétaires,Propriétaires actifs,Demandeurs,Demandeurs actifs,Fournisseur,Prescripteur,Attributs,Activité,Mailing,e-mailing,Magazine,Langue parlée 1,Langue parlée 2,Monnaie,Extranet,Contact lié,Situation familiale,Régime matrimonial,Nombre d'enfants,Site internet,Créé le,Mise à jour le,Commentaire
8751280,Immo Plus,Service DES VENTES123,Particulier,,Monsieur ,JOHNY,JAHN,,johnyjahn@citycable.ch,,0789139000,,,,,,,,,,,,,,,,chemin de l'ancien stand de fabrication de pied 10,,1018,Lausanne,Suisse,,,X,,,,,,Non abonné,Non abonné,Non abonné,français,,,X,,,,,,2018-08-28 14:52:32,2022-07-15 14:54:38,
```
