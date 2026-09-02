# API Design Notes

## Overview

This document summarizes practical considerations for designing maintainable REST APIs.

## Resource-Oriented Design

API endpoints should represent meaningful resources rather than actions whenever practical.

Examples:

- GET /users
- GET /users/{id}
- POST /users
- PATCH /users/{id}
- DELETE /users/{id}

## HTTP Methods

HTTP methods should be used consistently according to the operation being performed.

- GET — Retrieve data
- POST — Create a resource or initiate an operation
- PUT — Replace a resource
- PATCH — Partially update a resource
- DELETE — Remove a resource

## HTTP Status Codes

Responses should use appropriate HTTP status codes to communicate the result clearly.

Examples:

- 200 OK
- 201 Created
- 204 No Content
- 400 Bad Request
- 401 Unauthorized
- 403 Forbidden
- 404 Not Found
- 409 Conflict
- 500 Internal Server Error

## Error Handling

APIs should return predictable and useful error responses rather than inconsistent messages.

A consistent error structure can make APIs easier for clients to consume and troubleshoot.

## Security

API design should consider:

- Authentication
- Authorization
- Input validation
- Data protection
- Rate limiting
- Secure handling of sensitive information

## Consistency

Naming conventions, response structures, error formats, pagination approaches, and other API conventions should remain consistent across the system.

## Additional Considerations

Depending on the application, API design may also need to address:

- Pagination
- Filtering
- Sorting
- Versioning
- Documentation
- Logging
- Monitoring

## Evaluation Perspective

When evaluating AI-generated API guidance, I assess technical accuracy, completeness, practical usefulness, consistency, security awareness, and whether recommendations are appropriately qualified.

## Conclusion

Good API design should make an interface predictable, understandable, maintainable, and practical for its intended consumers.
