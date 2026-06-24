# Use Cases

# SmartDesk AI Platform

**Version:** 1.0

---

# UC-001 - User Login

## Primary Actor

User

## Description

The user logs into the platform using their email and password.

## Preconditions

* The user is registered.
* The account is active.

## Main Flow

1. User opens the login page.
2. User enters email and password.
3. System validates credentials.
4. System grants access.
5. Dashboard is displayed.

## Alternative Flow

* Invalid credentials.
* Account locked.

---

# UC-002 - Create Support Ticket

## Primary Actor

End User

## Description

The user creates a new support ticket.

## Preconditions

* User is authenticated.

## Main Flow

1. User selects "New Ticket".
2. User enters title and description.
3. User submits the request.
4. System creates the ticket.
5. Confirmation is displayed.

---

# UC-003 - Assign Ticket

## Primary Actor

Support Agent

## Description

Assign a ticket to a technician.

---

# UC-004 - Resolve Ticket

## Primary Actor

Support Agent

## Description

Close a resolved support ticket.

---

# UC-005 - AI Assistant

## Primary Actor

End User

## Description

Interact with the AI assistant to solve common issues.

---

# UC-006 - Dashboard

## Primary Actor

Administrator

## Description

View support metrics and KPIs.

---

# UC-007 - Manage Users

## Primary Actor

Administrator

## Description

Create, update and deactivate users.
