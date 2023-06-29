# Search - Publimmo CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search ID in your system |
| 16 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 6,25,26,27 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Contact ID this search is linked to |
| 7 | string | [Search Status](../values/search_status_id.md) | Search status |
| 35 | string | [Search Transaction Type](../values/search_transaction_type_id.md) | Property transaction type |
| 35 | string | [Property Category](../values/property_category_id.md) | Property category |
| 35 |  | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 8 | string | [Property Position](../values/property_position_id.md) | Semicolon separated list of property positions |
| 9 | string | [Property Furnishing](../values/property_furnishing_id.md) | Semicolon separated list of property furnishings |
| 10 | string | [Property Style](../values/property_style_id.md) | Semicolon separated list of property styles |
| 11 | string | [Property View](../values/property_view_id.md) | Semicolon separated list of property views |
| 12 | string | [Property Sonority](../values/property_sonority_id.md) | Semicolon separated list of property sonorities |
| 13 | string | [Property Space Type](../values/property_space_type_id.md) | Semicolon separated list of property space types |
| 35 | json | { "level": country|canton|district|zone|city|quarter, "name": string } | Search locations |
| 35 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search label |
| 31 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search private comment |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price min |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price max |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property area min |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property area max |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room min |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room max |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property bedroom min |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property bedroom max |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land min |
| 35 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land max |
| 34 | date | d.m.Y | d-m-Y | Y-m-d | Search update date |
| 34 |  |  | Property is new |
| 35 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is allowed to foreigners |
| 36 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Search is hidden in global matching |

## Sample

[search-publimmo.csv](../samples/search-publimmo.csv)
```
ID,Politesse,Nom,PrÃ©nom,Langue,eMail,Statut,Adresse,Adresse 2,Npa,LocalitÃ©,Pays,TÃ©lÃ©phone,Mobile,Evaluation,Courtier ID,Agence ID,Groupe ID,Type,Communication,SociÃ©tÃ©,Client Final,Nom 2,PrÃ©nom 2,eMail 2,eMail 3,eMail 4,Pays,Fax,TÃ©lÃ©phone 2,Remarques,Activer les relances,CrÃ©ation,Action,Filtre(s),,,
897216,"Madame, Monsieur",KARO,Philippe,fr,infodecaro@immochateau.ch,Actif,,,,,CH,,,,jacky@cfp-immo.ch,431742,0,Acheteur,eMail,Agence ImmobiliÃ¨re du ChÃ¢teau,,,,,,,CH,,,,Oui,15.12.2020,21.02.2022,Acheter | Commercial,"Acheter | Maison | TrÃ©lex, 4km",,,
```
