# Example REST API

A simple conceptual API for managing users.

## Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/users` | List users |
| GET | `/users/{id}` | Retrieve a user |
| POST | `/users` | Create a user |
| PATCH | `/users/{id}` | Update selected fields |
| DELETE | `/users/{id}` | Delete a user |

## Example Request

```http
GET /users/123
Accept: application/json

Example Response
{
  "id": 123,
  "name": "Example User",
  "status": "active"
}

Design Considerations

A production API would additionally require appropriate authentication, authorization, validation, error handling, logging, monitoring, documentation, and data-protection controls.

This example is intentionally simple and is intended to demonstrate API design concepts rather than represent a production implementation.


Commit:

```text
Add REST API example
