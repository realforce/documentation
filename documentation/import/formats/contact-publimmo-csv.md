# Contact - Publimmo CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact ID in your system |
| 2 | string | [Contact Title](../values/contact_title_id.md) | Contact title |
| 3 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact lastname |
| 4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact firstname |
| 5 | string | [Language](../values/language_id.md) | Contact language |
| 6,20,25,26,27 | json | { "notes": string, "value": string, "use_mailing": boolean, "is_main": boolean } | Comma separated list of emails |
| 7 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is archived |
| 8,9,10,11,12 | json | { "notes": string, "country_id": string, "line1": string, "line2": string, "line3": string, "city": string, "zip": string, "use_default": boolean } | Comma separated list of addresses |
| 13,14,15,30 | json | { "notes": string, "number": string, "type": mobile/landline, "is_main": boolean } | Comma separated list of phones |
| 16 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 19 | string | [Contact Type](../values/contact_type_id.md) | Comma separated list of contact types |
| 21 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact company name |
| 22 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is a direct client |
| 23 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact second lastname |
| 24 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact second firstname |
| 30 | string | [Country](../values/country_id.md) | Contact nationality |
| 31 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact private comment |
| 33 | datetime | YYYY-MM-DD hh:mm:ss | Contact creation date & time |
| 34 | datetime | YYYY-MM-DD hh:mm:ss | Contact update date & time |

## Sample

[contact-publimmo.csv](../samples/contact-publimmo.csv)
```
ID,Politesse,Nom,Prénom,Langue,eMail,Statut,Adresse,Adresse 2,Npa,Localité,Pays,Téléphone,Mobile,Evaluation,Courtier ID,Agence ID,Groupe ID,Type,Communication,Société,Client Final,Nom 2,Prénom 2,eMail 2,eMail 3,eMail 4,Pays,Fax,Téléphone 2,Remarques,Activer les relances,Création,Action,Filtre(s)
1148329,Madame et Monsieur,Loisel,loide,fr,ana.loisel759@gmail.com,Actif,bergholzweg,,8123,ebmatingen,CH,,0786643073,,945276,385384,585320,Acheteur,eMail,,,,,,,,CH,,,"Venu par: Homegate (821122) Bonjour,Ce bien m'intéresse.Meilleures salutations",Oui,24.06.2022,24.06.2022,"Acheter | Maison | Pièces min.: 6 | Prix maximum: 2'409'000.- | Crassier, 8km"

```
