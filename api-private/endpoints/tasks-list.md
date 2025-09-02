# Tasks - List
Fetch a list of tasks sorted by ID, accessible to the private API key.

- All string values can be NULL.
- Property details can be fetched from the Properties API endpoint.
- Promotion details can be fetched from the Promotions API endpoint.

## Endpoint
```
GET https://agency.realforce.ch/api/tasks/listall
```

## Request

#### Headers

| Header | Value        |
| :--- |:-------------|
| X-API-KEY | **_your API key_** |

#### Parameters

| Name             | Type              | Required | Description                                          |
|:-----------------|:------------------|:---------|:-----------------------------------------------------|
| per_page         | int               | yes      | Number of records to retrieve per page (max 50)      |
| page             | int               | yes      | Index of the page to retrieve                        |
| lang             | string            | yes      | Content languages in lower case: fr/en/it/de         |
| promotion.uuid[] | string (multiple) | no       | Filter on promotions UIDs                            |
| task_type_id[]   | int (multiple)    | no       | Filter on task types IDs                             |
| is_finished      | int               | no       | Filter on task finished status: 0 = false / 1 = true |
| create_from      | date YYYY-MM-DD             | no       | Filter on task creation date "from"                  |
| create_to        | date YYYY-MM-DD             | no       | Filter on task creation date "to"                    |

#### Task types

| ID  | Type        |
|:----|:------------|
| 5   | Rendez-vous | 
| 6   | Visite      |
| 9   | Mailing     |  
| 10  | Remise de brochure |         
| 12  | Activer publication sur portail |
| 13  | Désactiver publication sur portail |
| 14  | Appel téléphonique |
| 15  | Envoi d'email |
| 16  | Envoi de fax                    | 
| 17  | Envoi de courrier                |
| 18  | Signature                        |
| 20  | Autre                            |
| 21  | Estimation                       |
| 22  | Évènement                        |
| 23  | Offre reçue                      |
| 24  | Offre retirée                    |
| 25  | Offre refusée                    |
| 26  | Offre acceptée                   |
| 27  | Suivi                            |
| 28  | Message laissé sur le répondeur  |
| 29  | Intérêt communiqué par le client |
| 31  | Promesse d'achat              |
| 32  | Vente du bien                 |
| 33  | Location du bien              |
| 34  | Réponse négative du client    |
| 35  | SMS                           |
| 36  | Financement immobilier        |
| 37  | Etat des lieux                |
| 38  | Journée portes ouvertes       |
| 39  | Brochure ouverte              |
| 40  | Annonce publicitaire          |
| 41  | Alerte email                  |
| 42  | Communication au propriétaire |
| 43  | Prospection           |
| 44  | Visite annulée        |
| 45  | Relance par téléphone |




#### Sample
```
GET https://agency.realforce.ch/api/tasks/listall
?per_page=20
&page=3
&lang=fr
&promotion.uuid[]=1234
&promotion.uuid[]=5678
&task_type_id[]=5
&task_type_id[]=6
&is_finished=1
&create_from=2023-04-19
&create_to=2023-04-21
```


## Response
The API response follows the Hydra Core Vocabulary: http://www.hydra-cg.com/spec/latest/core/

#### Sample
```
{
 "@context": "/api/contexts/Task",
 "@id": "/api/tasks",
 "@type": "hydra:Collection",
 "hydra:member": [
   {
     "@id": "/api/tasks/1337",
     "@type": "Task",
     "id": 1337,
     "agency": {
       "@id": "/api/agencies/404",
       "@type": "Agency",
       "id": 404,
       "name": "Demo Agency"
     },
     "title": "Visite - Bureaux rénovés - REF123456 | Champel",
     "location": "Avenue de Champel 31",
     "dueDatetime": "2019-03-25T18:15:00+00:00",
     "endDatetime": "2019-03-25T19:00:00+00:00",
     "taskType": "Visite",
     "createdBy": {
       "@id": "/api/contacts/42",
       "@type": "Contact",
       "id": 42,
       "firstname": "Michael",
       "lastname": "Smith",
       "emails": [
         "michael.smith@myagency.example"
       ]
     },
     "createdDatetime": "2019-03-18T11:25:47+00:00",
     "finishedBy": {
       "@id": "/api/contacts/101",
       "@type": "Contact",
       "id": 101,
       "firstname": "Paul",
       "lastname": "Cook",
       "emails": [
         "paul.cook@myagency.example"
       ]
     },
     "finishedDatetime": "2019-03-25T20:00:00+00:00",
     "reminderDatetime": "2019-03-25T15:00:00+00:00",
     "personalNotes": "Ne pas appeler avant midi",
     "publicReport": "Troisième visite dans le quartier",
     "notesSentToContact": "Visite confirmée une semaine à l'avance",
     "important": true,
     "finished": true,
     "sendNotesToContact": true,
     "sendInvitationToAssignee": true,
     "sendInvitationToParticipant": true,
     "published": true,
     "editableByOthers": true,
     "systemGenerated": false,
     "private": false,
     "hideInReports": true,
     "sendTaskToOwner": true,
     "taskCreatedFromGlobalMatching": false,
     "isEmailed": true,
     "contactAddressee": [
       {
         "@id": "/api/contacts/301",
         "@type": "Contact",
         "id": 301,
         "firstname": "John",
         "lastname": "Doe",
         "emails": [
           "john.doe@mail.example"
         ]
       },
       {
         "@id": "/api/contacts/302",
         "@type": "Contact",
         "id": 302,
         "firstname": "Jane",
         "lastname": "Doe",
         "emails": [
           "jane.doe@mail.example"
         ]
       }
     ],
     "contactAssignee": [
       {
         "@id": "/api/contacts/101",
         "@type": "Contact",
         "id": 101,
         "firstname": "Paul",
         "lastname": "Cook",
         "emails": [
           "paul.cook@myagency.example"
         ]
       }
     ],
     "contactParticipant": [
       {
         "@id": "/api/contacts/42",
         "@type": "Contact",
         "id": 42,
         "firstname": "Michael",
         "lastname": "Smith",
         "emails": [
           "michael.smith@myagency.example"
         ]
       }
     ],
     "promotion": [
       {
         "@id": "/api/promotions/444",
         "@type": "Promotion",
         "uuid": 1234
       },
       {
         "@id": "/api/promotions/333",
         "@type": "Promotion",
         "uuid": 5678
       }
     ],
     "property": [
       {
         "@id": "/api/properties/1000",
         "@type": "Property",
         "uuid": 1000
       },
       {
         "@id": "/api/properties/2000",
         "@type": "Property",
         "uuid": 2000
       },
       {
         "@id": "/api/properties/9999",
         "@type": "Property",
         "uuid": 9999
       }
     ]
   }
 ],
 "hydra:totalItems": 123,
 "hydra:view": {
   "@id": "/api/tasks?page=1",
   "@type": "hydra:PartialCollectionView",
   "hydra:first": "/api/tasks?page=1",
   "hydra:last": "/api/tasks?page=123",
   "hydra:next": "/api/tasks?page=2"
 },
 "hydra:search": {
   "@type": "hydra:IriTemplate",
   "hydra:template": "/api/tasks{?properties[]}",
   "hydra:variableRepresentation": "BasicRepresentation",
   "hydra:mapping": [
     {
       "@type": "IriTemplateMapping",
       "variable": "properties[]",
       "property": null,
       "required": false
     }
   ]
 }
}
```
