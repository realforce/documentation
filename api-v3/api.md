# 📘 REALFORCE API

## 📑 Table of Contents
- [🔹 Introduction](#-introduction)
- [🔑 Authentication](#-authentication)
- [📇 Contact](#-contact)
- [📌 Leads](#-leads)
- [🏠 Property](#-property)
- [🏢 Promotion](#-promotion)
- [📋 Notes générales](#-notes-générales)

---

## 🔹 Introduction

- **Base URL** : `https://crm.realforce.ch/api/v3/`
- **Supported format / Format supporté** : `JSON`
- **Version** : `1.0`
- **Status / Statut** : `Stable`
- **Content-Type** : `application/json`

---

## 🔑 Authentication

| Header    | Value              |
|:----------|:-------------------|
| X-API-KEY | **_your API key_** |

### Response

## 🔖 HTTP Status Codes

| Code | Status                | Description (EN)                             |
|------|-----------------------|----------------------------------------------|
| 200  | OK                    | Request succeeded                            |
| 201  | Created               | Resource successfully created                |
| 204  | No Content            | Success, no content returned                 |
| 400  | Bad Request           | Invalid or missing parameters                |
| 401  | Unauthorized          | Missing or invalid authentication (API key)  |
| 403  | Forbidden             | Authenticated but insufficient permissions   |
| 404  | Not Found             | Resource does not exist                      |
| 409  | Conflict              | Conflict with current state (e.g. duplicate) |
| 500  | Internal Server Error | Generic server-side error                    |


# Contact

#### Endpoint

```
GET /api/v3/contact/list
POST /api/v3/contact/add
```

### Parameters
| Name     | Type    | Required | Description                          |
|----------|---------|----------|--------------------------------------|
| per_page | int     | yes      | Number of records per page (max 100) |
| page     | int     | yes      | Page number                          |
| archived | boolean | no       | `true`, `false`, or empty for all    |

## Response

```body
Body
{
  "contact_lastName": "Jean",
  "contact_firstName": "Dupont",
  "email_visible": "jean.dupont@example.com",
  "contact_mobile": "+41791234567",
  "contact_type": "Courtier",
}
```

# Leads

#### Endpoint

```
GET /api/v3/leads/list
POST /api/v3/leads/add
```

#### Parameters
| Name     | Type   | Required | Description                                      |
|:---------|:-------|:---------|:-------------------------------------------------|
| per_page | int    | yes      | Number of records to retrieve per page (max 100) |
| page     | int    | yes      | Index of the page to retrieve                    |
| source   | string | no       | name of source or nothing for all records        |

## Response

```body
Body
{
  "contact_lastName": "Jean",
  "contact_firstName": "Dupont",
  "email_visible": "jean.dupont@example.com",
  "contact_mobile": "+41791234567",
  "contact_type": "Courtier",
}
```
# Property

#### Endpoint

```
GET /api/v3/property/list
GET /api/v3/property/details?id={id}
POST /api/v3/property/add
```

#### Parameters
| Name       | Type     | Required | Description                                                                                                      |
|:-----------|:---------|:---------|:-----------------------------------------------------------------------------------------------------------------|
| per_page   | int      | yes      | Number of records to retrieve per page (max 100)                                                                 |
| page       | int      | yes      | Index of the page to retrieve                                                                                    |
| archived   | boolean  | no       | true/false or nothing for all records                                                                            |
| lang       | string   | yes      | Content languages in lower case (fr, en, it, de). Multiple languages can be retrieved using the "pipe" separator |
| status     | string[] | no       | status or nothing                                                                                                |
| categories | string[] | no       | status or nothing                                                                                                |

| Name | Type     | Required | Description               |
|:-----|:---------|:---------|:--------------------------|
| id   | int      | yes      | Retrieve details property |

## Response


# Promotion

#### Endpoint

```
GET /api/v3/promotion/list
GET /api/v3/promotion/details?id={id}
POST /api/v3/promotion/add
```

#### Parameters
| Name     | Type    | Required | Description                                                                                                      |
|:---------|:--------|:---------|:-----------------------------------------------------------------------------------------------------------------|
| per_page | int     | yes      | Number of records to retrieve per page (max 100)                                                                 |
| page     | int     | yes      | Index of the page to retrieve                                                                                    |
| lang     | string  | yes      | Content languages in lower case (fr, en, it, de). Multiple languages can be retrieved using the "pipe" separator |
| archived | boolean | no       | true/false or nothing for all records                                                                            |

| Name | Type     | Required | Description                |
|:-----|:---------|:---------|:---------------------------|
| id   | int      | yes      | Retrieve details promotion |

## Response




# Estimation time

### Use add quick or not for property and contact?

| Endpoint                                                 | estimation (days) | order |
|:---------------------------------------------------------|:------------------|:------|
| GET /api/v3/agencies/{agencyId}/contacts                 | 3                 | 1     |
| POST /api/v3/agencies/{agencyId}/contacts                | 2                 | 2     |
| GET /api/v3/agencies/{agencyId}/leads                    | 1                 | 3     |
| POST /api/v3/agencies/{agencyId}/leads                   | 1                 | 4     |
| PUT /api/v3/agencies/{agencyId}/contacts/{contactId}     | 1                 | 5     |
| GET /api/v3/agencies/{agencyId}/contacts/{contactId}     | 2                 | 6     |
| GET /api/v3/agencies/{agencyId}/properties               | 1                 | 7     |
| GET /api/v3/agencies/{agencyId}/properties/{propertyId}  | 2                 | 8     |
| POST /api/v3/agencies/{agencyId}/properties              | 2                 | 9     |
| GET /api/v3/agencies/{agencyId}/promotions               | 1                 | 10    |
| GET /api/v3/agencies/{agencyId}/promotions/{promotionId} | 1                 | 11    |
| POST /api/v3/agencies/{agencyId}/promotions              | 1                 | 12    |
