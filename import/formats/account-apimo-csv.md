# Account - Apimo CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 3,4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User ID in your system |
| 2 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | User is active |
| 3 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User firstname |
| 4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User lastname |
| 5 | string | [Account Role](../values/account_role_id.md) | User type |
| 8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User email used as login in RealForce |

## Sample

[account-apimo.csv](../samples/account-apimo.csv)
```
Référence,Actif,Prénom,Nom de famille,Profil,Agence,Langue,e-mail,Mobile,Téléphone,Connexion,Mot de passe
25021,1,Service,DES VENTES123,Gérant,11580,fr,servicedesventes@immo-plus123.ch,,41788094600 ,23/11/22,21/01/21
```
