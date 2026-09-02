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
```
## Example Response
```JSON
{
  "id": 123,
  "name": "Example User",
  "status": "active"
}
```
## Example Create Request
```http
POST /users
Content-Type: application/json

{
  "name": "Example User",
  "status": "active"
}
```
## Example Create Response
```http
HTTP/1.1 201 Created
Content-Type: application/json
```
```json
{
  "id": 124,
  "name": "Example User",
  "status": "active"
}
```
## Error Response Example
```json
{
  "error": {
    "code": "USER_NOT_FOUND",
    "message": "The requested user could not be found."
  }
}
```
## Design Considerations
A production API would additionally require appropriate:

- Authentication
- Authorization
- Input validation
- Error handling
- Logging
- Monitoring
- Rate limiting
- Documentation
- Data protection

The exact implementation would depend on the application's requirements and architecture.

Purpose

This example is intentionally simple. It demonstrates API design concepts rather than representing a production implementation.

It is included as an independent technical portfolio example.


