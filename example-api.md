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

