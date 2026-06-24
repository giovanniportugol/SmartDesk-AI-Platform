# Database Design

# SmartDesk AI Platform

**Version:** 1.0

**Status:** Draft

---

# 1. Overview

The SmartDesk AI Platform uses PostgreSQL as its primary relational database.

The database is designed to support authentication, ticket management, AI interactions, notifications, and reporting.

---

# 2. Main Entities

## User

Stores user account information.

Attributes:

* id
* full_name
* email
* password_hash
* role_id
* created_at
* updated_at

---

## Role

Defines user permissions.

Attributes:

* id
* name
* description

Examples:

* Administrator
* Support Agent
* End User

---

## Ticket

Stores support requests.

Attributes:

* id
* title
* description
* status
* priority
* category_id
* created_by
* assigned_to
* created_at
* updated_at

---

## Category

Groups tickets by subject.

Examples:

* Hardware
* Software
* Network
* Account Access
* AI Support

---

## Message

Stores conversations related to a ticket.

Attributes:

* id
* ticket_id
* user_id
* message
* created_at

---

## Notification

Stores system notifications.

Attributes:

* id
* user_id
* title
* message
* is_read
* created_at

---

# 3. Relationships

* One Role can have many Users.
* One User can create many Tickets.
* One User can be assigned to many Tickets.
* One Category can contain many Tickets.
* One Ticket can contain many Messages.
* One User can receive many Notifications.

---

# 4. Future Improvements

Future database enhancements may include:

* Audit logs
* File attachments
* AI conversation history
* Customer satisfaction surveys
* Knowledge base articles
