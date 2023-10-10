# Search - Ohuho CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search ID in your system |
| 26 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 1 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Contact ID this search is linked to |
| 23 | string | [Search Transaction Type](../values/search_transaction_type_id.md) | Property transaction type |
| 23 | string | [Property Category](../values/property_category_id.md) | Property category |
| 23 | json | { "level": country|canton|district|zone|city|quarter, "name": string } | Search locations |
| 23 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price min |
| 23 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price max |
| 23 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property area min |
| 21 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room min |
| 22 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room max |

## Sample

[search-ohuho.csv](../samples/search-ohuho.csv)
```
idPerson,Civilite,Nom,Prenom,Statut,Actif,Societe,Adresse,Adresse2,Etranger,Pays,Region,Localite,ZipCode,Telephone,Mobile,Fax,EMail,EMail2,EMail3,Communication,Annotations,Recherches,Activites,Objects,idCourtier,Type
13408,Monsieur,Bie,Jean,A relancer,1,,,,0,,,,,,#ERROR!,,jf.b@bluewin.ch,,,fr,"recherche chalet 4.5-5.5 pièces ou appartement en pleins centre 3.5 pièces ou plus. aime le vieux bois et rêve d'avoir un bien au mer de glace.  budget 1'000'000 - 1'600'000  accessibilité important  A un chalet de 2021, à vendre en cas d'achat d'un autre bien.","Vente, Appartement, 1996 Basse-Nendaz, pieces min: 3.5, pieces max: 5.5, prix min: 1, prix max: 1600000, surface min: 80
Vente, Appartement, 1997 Haute-Nendaz, pieces min: 3.5, pieces max: 5.5, prix min: 1, prix max: 1600000, surface min: 80
Vente, Appartement, 1997 Siviez (Nendaz), pieces min: 3.5, pieces max: 5.5, prix min: 1, prix max: 1600000, surface min: 80
","Visite, objet: 11171, ref: ALP-11171, date: 2023-05-24 00:00:00, delai: 2023-05-24 00:00:00, commentaire: Visite avec M. seul. Fribourgeois, fromager, sa femme ingénieur agro. Habitent dans le canton de FR mais ont déjà un chalet en dessous de Nendaz, construit en 2021. Ils aiment bouger, 2e achat sur Nendaz déjà. Sa femme aime bcp ce complex de la mer de glace et rêve d'y avoir un appart. Celui visité a du bois trop clair, elle aime le vieux bois. Si un bien ce libère avec du vieux bois, 3,5p - 4,5p le relancer sans faute. , Terminé
Visite, objet: 11100, ref: ALP-11100, date: 2023-05-24 00:00:00, delai: 2023-05-24 00:00:00, commentaire: Visite avec M. Ce bien lui plait bcp avec le vieux bois et la grande terrasse, aime recevoir. Il va en discuter avec sa femme et revient vers moi si intéressé pour une 2e visite. Si ils prennent ce bien ils nous donneraient le mandat pour vendre leur chalet construit en 2021. Le tenir informé de la situation. , Terminé
Dossier envoyé par mail, objet: 11100, ref: ALP-11100, date: 2023-05-23 00:00:00, delai: 2023-05-28 00:00:00, À traiter
Dossier envoyé par mail, objet: 11171, ref: ALP-11171, date: 2023-05-23 00:00:00, delai: 2023-05-28 00:00:00, À traiter
Appeler pour relancer, date: 2023-01-05 00:00:00, delai: 2023-03-01 00:00:00, À traiter
Visite, objet: 9290, ref: ALP-9290, date: 2021-08-13 00:00:00, delai: 2021-08-17 00:00:00, Terminé
",,CLEEDO1024,Acheteur
```
