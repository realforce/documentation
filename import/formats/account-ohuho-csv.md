# Account - Ohuho CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User ID in your system |
| 2 | string | [Account Role](../values/account_role_id.md) | User type |
| 3 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User email used as login in RealForce |
| 4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User password |
| 5 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User firstname |
| 6 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User lastname |
| 7 | date | d.m.Y | d-m-Y | Y-m-d | User expiry date |
| 8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | User private comment |
| 9 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | User is active |

## Sample

[account-ohuho.csv](../samples/account-ohuho.csv)
```
ID,accountTypeId,email,password,firstname,lastname,expiryDate,comment,isActive
IDUSER001,admin,import-admin-001@realforce.ch,mysecretpassword,Admino,Importo,,Ceci est un compte de test,TRUE
IDUSER002,courtier,import-courtier-001@realforce.ch,ab1234,Courtiero,Importo,2022-06-01,Ceci est un autre compte de test,TRUE
```
