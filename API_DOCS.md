# 📚 Smart Leads Dashboard - API Documentation

## 📌 Overview
This document provides details of all backend APIs used in the Smart Leads Dashboard project.  
The backend is built using **Node.js, Express, and TypeScript**, following RESTful API standards.

---

## 🌐 Base URL

Local:
```
[http://localhost:5000/api/v1]

```
Production:
```
https://github.com/poojakumar2004/Smart-Lead-Dashboard

````

---

## 🔐 Authentication APIs

### 1. Register User
**POST** `/auth/register`

**Request Body:**
```json
{
  "name": "pooja",
  "email": "pooja@gmail.com",
  "password": "1162"
}
````

**Response:**

```json
{
  "message": "User registered successfully",
  "token": "jwt_token_here"
}
```

---

### 2. Login User

**POST** `/auth/login`

**Request Body:**

```json
{
  "email": "pooj@gmail.com",
  "password": "1162"
}
```

**Response:**

```json
{
  "message": "Login successful",
  "token": "jwt_token_here"
}
```

---

## 📊 Leads APIs

### 1. Get All Leads

**GET** `/leads`

**Response:**

```json
[
  {
    "id": "1",
    "name": "pooja",
    "email": "pooja@gmail.com",
    "status": "New"
  }
]
```

---

### 2. Create Lead

**POST** `/leads`

**Request Body:**

```json
{
  "name": "pooja",
  "email": "pooja@gmail.com",
  "status": "New"
}
```

---

### 3. Update Lead

**PUT** `/leads/:id`

---

### 4. Delete Lead

**DELETE** `/leads/:id`

---

## 🔎 Saved Filters APIs (if used)

### GET `/filters`

Get saved filters for user

### POST `/filters`

Create a new filter

### DELETE `/filters/:id`

Delete a filter

---

## 📁 Bulk Import / Export APIs (if used)

### POST `/leads/import`

Import leads in bulk

### GET `/leads/export`

Export leads data

---

## 🔑 Authentication Method

All protected routes require JWT token in headers:

```
Authorization: Bearer <token>
```

---

## ⚠️ Error Handling

### 400 Bad Request

```json
{
  "error": "Invalid request data"
}
```

### 401 Unauthorized

```json
{
  "error": "Access denied. No token provided"
}
```

### 404 Not Found

```json
{
  "error": "Resource not found"
}
```

### 500 Server Error

```json
{
  "error": "Internal server error"
}
```

---

## 🔄 API Flow Example

1. Register user → `/auth/register`
2. Login user → get JWT token
3. Use token in headers
4. Access `/leads` APIs

## 🚀 Notes

* All APIs follow REST standards
* Data is exchanged in JSON format
* Authentication uses JWT tokens

# 🎯 DONE

This is **fully internship-ready API documentation**.

