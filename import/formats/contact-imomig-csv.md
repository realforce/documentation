# Contact - Imomig CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 3 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact ID in your system |
| 12 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact firstname |
| 11 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact lastname |
| 56 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact second firstname |
| 55 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact second lastname |
| 37 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID that created the contact |
| 8 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID that updated the contact |
| 16 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact company name |
| 11 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact private comment |
| 12 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Contact ranking from 1 to 3 |
| 4 | string | [Contact Type](../values/contact_type_id.md) | Semicolon separated list of contact types |
| 24,25,66 | json | { "notes": string, "number": string, "type": mobile/landline, "is_main": boolean } | Semicolon separated list of phones |
| 29,30 | json | { "notes": string, "value": string, "is_use_mailing": boolean, "is_main": boolean } | Semicolon separated list of emails |
| 18,19,20,21,22,23 | json | { "notes": string, "country_id": string, "line1": string, "line2": string, "line3": string, "city": string, "zip": string, "use_default": boolean } | Semicolon separated list of addresses |
| 17 | string | [Pipeline Stage](../values/pipeline_stage_id.md) | Contact pipeline stage |
| 18 | date | d.m.Y | d-m-Y | Y-m-d | Contact pipeline date |
| 14 | date | d.m.Y | d-m-Y | Y-m-d | Contact birthdate |
| 5 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Contact creation date & time |
| 7 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Contact update date & time |
| 37 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 9 | string | [Contact Title](../values/contact_title_id.md) | Contact title |
| 27 | string | [Greeting](../values/greeting_id.md) | Contact greeting |
| 38 | string | [Language](../values/language_id.md) | Contact language |
| 29 | string | [Visibility](../values/visibility_id.md) | Contact visibility/sharing |
| 48 | string | [Origin](../values/origin_id.md) | Contact origin |
| 35 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is archived |

## Sample

[contact-imomig.csv](../samples/contact-imomig.csv)
```
id,firstname,lastname,firstname2,lastname2,createAccountId,updateAccountId,company,employment,bank,comment,ranking,contactTypeIds,phones,emails,addresses,pipelineStageId,pipelineStageDate,birthdayDate,createDatetime,updateDatetime,lastContactDate,brokerAccountId,brokerSaleAccountId,brokerRentAccountId,titleId,greetingId,languageId,visibilityId,nationalityId,familyId,childrenId,originId,intermediaryAccountId,isArchived,isVip,isDirectClient,isHideContactOnMls,isAnonymous,isVisibleOnWebsite,linkedin,instagram,facebook,twitter
IDCONTACT000001,John,Doe,Johanna,Doe,IDUSER001,,Testo Real Estato,CEO,UBS,"Ceci est un contact de test, on place les employés de l'agence en premier",3,Courtier Vente,"{""number"":""079 333 4444"", ""notes"":""Natel perso"", ""type"": ""mobile"", ""is_main"": ""true""}; {""number"":""022 111 2222"", ""notes"":""Pro"", ""type"": ""landline"", ""is_main"": ""false""}","{""value"":""john-doe@testorealestato.ch"", ""notes"":""Email pro"", ""is_use_mailing"": ""true"", ""is_main"": ""true""}; {""value"":""john-doe@gmail.com"", ""notes"":""Email perso"", ""is_use_mailing"": ""false"", ""is_main"": ""false""}",,,,1980-12-01,2020-01-01 09:00:00,,,IDUSER001,,,Monsieur,Cher Monsieur,fr,Agence,Suisse,Célibataire,0,,,FALSE,FALSE,FALSE,FALSE,FALSE,TRUE,https://linkedin.com/john-doe,https://instagram.com/john-doe,https://facebook.com/john-doe,https://twitter.com/john-doe
IDCONTACT000002,Julia,Smisseta,,,IDUSER002,IDUSER002,,,,"Ceci est un contact de test, c'est un client de John Doe.",1,Acheteur; Locataire,"{""number"":""0791231234"", ""notes"":"""", ""type"": ""mobile"", ""is_main"": ""true""}","{""value"":""julia.lacliente@gmail.com"", ""notes"":"""", ""is_use_mailing"": ""true"", ""is_main"": ""true""}","{""country_id"":""Suisse"", ""notes"":""Addresse pro"", ""line1"": ""Rue de la gare 1"", ""line2"": ""Les bureaux du futur"", ""line3"": ""Bâtiment A"", ""city"": ""Carouge"", ""zip"": ""1207"", ""use_default"": ""true""}",Biens envoyés,2021-04-06,1972-08-24,2021-03-21 17:24:02,2021-04-06 10:54:37,2021-04-06,IDUSER002,IDUSER002,IDUSER002,Madame,Chère Madame,fr,Agence,Suisse,Marié(e),2,Site internet agence,IDUSER002,FALSE,TRUE,TRUE,FALSE,FALSE,TRUE,,,,
```
