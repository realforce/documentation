# Contact - Realforce CSV

## Description

| Column | Type | Format | Description |
| :--- | :--- | :--- | :--- |
| 1 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact ID in your system |
| 2 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact firstname |
| 3 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact lastname |
| 4 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact second firstname |
| 5 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact second lastname |
| 6 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID that created the contact |
| 7 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID that updated the contact |
| 8 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact company name |
| 9 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact employment |
| 10 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact bank name |
| 11 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact private comment |
| 12 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Contact ranking from 1 to 3 |
| 13 | string | [Contact Type](../values/contact_type_id.md) | Semicolon separated list of contact types |
| 14 | json | { "notes": string, "number": string, "type": mobile/landline, "is_main": boolean } | Semicolon separated list of phones |
| 15 | json | { "notes": string, "value": string, "is_use_mailing": boolean, "is_main": boolean } | Semicolon separated list of emails |
| 16 | json | { "notes": string, "country_id": string, "line1": string, "line2": string, "line3": string, "city": string, "zip": string, "use_default": boolean } | Semicolon separated list of addresses |
| 17 | string | [Pipeline Stage](../values/pipeline_stage_id.md) | Contact pipeline stage |
| 18 | date | d.m.Y | d-m-Y | Y-m-d | Contact pipeline date |
| 19 | date | d.m.Y | d-m-Y | Y-m-d | Contact birthdate |
| 20 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Contact creation date & time |
| 21 | datetime | d.m.Y H:i:s | d-m-Y H:i:s | Y-m-d H:i:s | Contact update date & time |
| 22 | date | d.m.Y | d-m-Y | Y-m-d | Contact last communication date |
| 23 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the main broker in charge |
| 24 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the sale broker in charge |
| 25 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the rental broker in charge |
| 26 | string | [Contact Title](../values/contact_title_id.md) | Contact title |
| 27 | string | [Greeting](../values/greeting_id.md) | Contact greeting |
| 28 | string | [Language](../values/language_id.md) | Contact language |
| 29 | string | [Visibility](../values/visibility_id.md) | Contact visibility/sharing |
| 30 | string | [Country](../values/country_id.md) | Contact nationality |
| 31 | string | [Family](../values/family_id.md) | Contact family |
| 32 | integer | [Number](https://en.wikipedia.org/wiki/Integer) | Contact number of children |
| 33 | string | [Origin](../values/origin_id.md) | Contact origin |
| 34 | string | [UID](https://en.wikipedia.org/wiki/Unique_identifier) | User ID of the intermediary broker |
| 35 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is archived |
| 36 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is VIP |
| 37 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is a direct client |
| 38 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is hidden on MLS |
| 39 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is anonymous |
| 40 | boolean | [Boolean](https://en.wikipedia.org/wiki/Boolean_data_type) | Contact is visible on website |
| 41 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact LinkedIn URL |
| 42 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact Instagram URL |
| 43 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact Facebook URL |
| 44 | string | [String](https://en.wikipedia.org/wiki/String_(computer_science)) | Contact Twitter URL |

## Sample

[contact-realforce.csv](../samples/contact-realforce.csv)
```
id,firstname,lastname,firstname2,lastname2,createAccountId,updateAccountId,company,employment,bank,comment,ranking,contactTypeIds,phones,emails,addresses,pipelineStageId,pipelineStageDate,birthdayDate,createDatetime,updateDatetime,lastContactDate,brokerAccountId,brokerSaleAccountId,brokerRentAccountId,titleId,greetingId,languageId,visibilityId,nationalityId,familyId,childrenId,originId,intermediaryAccountId,isArchived,isVip,isDirectClient,isHideContactOnMls,isAnonymous,isVisibleOnWebsite,linkedin,instagram,facebook,twitter
IDCONTACT000001,John,Doe,Johanna,Doe,IDUSER001,,Testo Real Estato,CEO,UBS,"Ceci est un contact de test, on place les employés de l'agence en premier",3,Collègue,"{""number"":""079 333 4444"", ""notes"":""Natel perso"", ""type"": ""mobile"", ""is_main"": ""true""}; {""number"":""022 111 2222"", ""notes"":""Pro"", ""type"": ""landline"", ""is_main"": ""false""}","{""value"":""john-doe@testorealestato.ch"", ""notes"":""Email pro"", ""is_use_mailing"": ""true"", ""is_main"": ""true""}; {""value"":""john-doe@gmail.com"", ""notes"":""Email perso"", ""is_use_mailing"": ""false"", ""is_main"": ""false""}",,,,1980-12-01,2020-01-01 09:00:00,,,IDUSER001,,,Monsieur,Cher Monsieur,fr,Agence,Suisse,Célibataire,0,,,FALSE,FALSE,FALSE,FALSE,FALSE,TRUE,https://linkedin.com/john-doe,https://instagram.com/john-doe,https://facebook.com/john-doe,https://twitter.com/john-doe
IDCONTACT000002,Julie,Smitho,,,IDUSER002,IDUSER002,,,,"Ceci est un contact de test, c'est un client de John Doe.",1,Acheteur; Locataire,"{""number"":""0791231234"", ""notes"":"""", ""type"": ""mobile"", ""is_main"": ""true""}","{""value"":""julia.lacliente@gmail.com"", ""notes"":"""", ""is_use_mailing"": ""true"", ""is_main"": ""true""}","{""country_id"":""Suisse"", ""notes"":""Addresse pro"", ""line1"": ""Rue de la gare 1"", ""line2"": ""Les bureaux du futur"", ""line3"": ""Bâtiment A"", ""city"": ""Carouge"", ""zip"": ""1207"", ""use_default"": ""true""}",Biens envoyés,2021-04-06,1972-08-24,2021-03-21 17:24:02,2021-04-06 10:54:37,2021-04-06,IDUSER002,IDUSER002,IDUSER002,Madame,Chère Madame,fr,Agence,Suisse,Marié(e),2,Site internet agence,IDUSER002,FALSE,TRUE,TRUE,FALSE,FALSE,TRUE,,,,
```
