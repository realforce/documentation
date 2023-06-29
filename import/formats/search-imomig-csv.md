# Search - Imomig CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search ID in your system |
| 35 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 1 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | Contact ID this search is linked to |
| 80 | string | [Search Status](../values/search_status_id.md) | Search status |
| 88 | string | [Search Transaction Type](../values/search_transaction_type_id.md) | Property transaction type |
| 84 | string | [Property Category](../values/property_category_id.md) | Property category |
| 84 |  | [Property Subcategory](../values/property_subcategory_id.md) | Property subcategory |
| 86 | json | { "level": country|canton|district|zone|city|quarter, "name": string } | Search locations |
| 79 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search label |
| 145 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Search private comment |
| 89 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price min |
| 90 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property price max |
| 106 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property area min |
| 107 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property area max |
| 98 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room min |
| 99 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property room max |
| 101 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property bedroom min |
| 102 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property bedroom max |
| 108 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land min |
| 109 | float | [Float](https://en.wikipedia.org/wiki/Decimal) | Property land max |
| 83 | date | d.m.Y | d-m-Y | Y-m-d | Search update date |
| 143 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Property is allowed to foreigners |

## Sample

[search-imomig.csv](../samples/search-imomig.csv)
```
id,Sorte de contact,Date d'inscription,Enregistré par,Date modification,Modifié par,Type contact,Type de contact supplémentaire,Nom,Prénom,Nom d'utilisateur,Date naissance,Titre,Société,Profession,Adresse,Complément d'adresse,Case postale,NPA,Ville,Pays,Téléphone,Mobile,Fax,Téléphone prof.,Téléphone directe,E-mail,Email 2,Etat civil,Réf.,Intitulé de correspondance,Préférence de correspondance,Statut,Agence principale,Courtiers,Langue de correspondance,Langues parlées,Revenu annuel,Taille du ménage,Nombre d'enfants,Type d'habitation actuelle,Usage nouvel objet,Site Internet,Remarques agent,Remarque client,Provenance,Type,Financement connu,L'acheteur sera financé par,Sorte de contact 2,Enregistré par 2,Modifié par 2,Nom contact 2,Prénom contact 2,Date naissance contact 2,Société contact 2,Profession 2,Adresse contact 2,"Complément d'adresse, contact 2",Case postale contact 2,NPA contact 2,Ville contact 2,Téléphone 2,Mobile 2,Fax 2,Téléphone prof. 2,Téléphone direct 2,Email contact 2,Deuxième email contact 2,Etat civil 2,Réf. 2,Intitulé de correspondance 2,Remarques agent 2,Provenance 2,Type 2,Langue,Langues parlées,Site Internet 2,Nom du filtre,Statut du filtre,Responsable du filtre,Date d'insertion du filtre,Date de modification du filtre,Catégorie,Région,Localités à inclure dans la recherche,Localités à exclure de la recherche,Type,Prix de,Prix à,Monnaie,Prix/m² de,Prix/m² à,Période de prix,Charges,Equipé,Résidence secondaire,Pièces de,Pièce à,Chambre de,Chambre à,Nombre de WC de,Nombre de WC à,Nombre de salles de bain de,Nombre de sanitaires à,Surface de,Surface à,Surface terrain de,Surface terrain à,Volume de,Volume à,Rendement brut de,Rendement brut à,Rendement net de,Rendement net à,Surface totale de,Surface totale à,Surface utile de,Surface utile à,Nombre de parcelles de,Nombre de parcelles à,Surface constructible de,Surface constructible à,Nombre de place de parc int. de,Nombre de place de parc int. à,Nombre de place de parc ext. de,Nombre de place de parc ext. à,Hauteur plafond de,Hauteur plafond à,Charge maximum sur la dalle [kg] de,Charge maximum sur la dalle [kg] à,Nbr. logements de,Nbr. logements à,Nombre de locaux admin. de,Nombre de locaux admin. à,Nbr. commerces de,Nbr. commerces à,Etat locatif brut de,Etat locatif brut à,Etat locatif net de,Etat locatif net à,Date limite de recherche,Vente aux étrangers,Remarques agent,Commentaires
2974387,Acheteur,15.05.2019,,15.05.2019,,Monsieur,,javlot,Loic,,,,,,,,,,,,,,,,,,,,,Monsieur Javlot,,Auto-archivé,Veyrat-Sarasin SA,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,"Madame, Monsieur",,,,,,,,,,,,,,,,,,,,,,,,Oui,Oui,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
```
