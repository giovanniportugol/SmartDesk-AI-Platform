# API Documentation

# SmartDesk AI Platform

**Version:** 1.0

**Status:** Draft

---

# Overview

The SmartDesk AI Platform exposes a RESTful API that enables communication between the frontend, backend, and external services.

Base URL:

```text
/api/v1
```

---

# Authentication

## POST /auth/login

Authenticates a user.

### Request

```json
{
  "email": "user@example.com",
  "password": "password123"
}
```

### Response

```json
{
  "token": "jwt_token",
  "user": {
    "id": 1,
    "name": "John Doe",
    "role": "Support Agent"
  }
}
```

---

## POST /auth/logout

Ends the authenticated session.

---

# Tickets

## GET /tickets

Returns all tickets available to the authenticated user.

---

## GET /tickets/{id}

Returns the details of a specific ticket.

---

## POST /tickets

Creates a new support ticket.

---

## PUT /tickets/{id}

Updates an existing ticket.

---

## DELETE /tickets/{id}

Deletes a ticket (Administrator only).

---

# Users

## GET /users

Returns the list of users.

---

## POST /users

Creates a new user.

---

## PUT /users/{id}

Updates user information.

---

## DELETE /users/{id}

Deactivates a user.

---

# AI Assistant

## POST /ai/chat

Sends a message to the AI assistant.

### Request

```json
{
  "message": "How can I reset my password?"
}
```

### Response

```json
{
  "answer": "To reset your password..."
}
```

---

# Status Codes

| Code | Description           |
| ---- | --------------------- |
| 200  | OK                    |
| 201  | Created               |
| 400  | Bad Request           |
| 401  | Unauthorized          |
| 403  | Forbidden             |
| 404  | Not Found             |
| 500  | Internal Server Error |
