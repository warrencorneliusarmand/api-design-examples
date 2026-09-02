# API Design Notes

## Overview

This document summarizes practical considerations for designing maintainable REST APIs.

## Core Principles

### Resource-Oriented Design

API endpoints should represent meaningful resources rather than actions whenever practical.

Examples:

- `GET /users`
- `GET /users/{id}`
- `POST /users`

### HTTP Methods

Use HTTP methods consistently according to the operation being performed.

- GET — Retrieve data
- POST — Create a resource or initiate an operation
- PUT — Replace a resource
- PATCH — Partially update a resource
- DELETE — Remove a resource

### Status Codes

Responses should use appropriate HTTP status codes to communicate results clearly.

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

### Error Handling

APIs should return predictable and useful error responses rather than inconsistent messages.

### Security

API design should consider authentication, authorization, input validation, data protection, rate limiting, and secure handling of sensitive information.

### Consistency

Naming conventions, response structures, error formats, and pagination approaches should remain consistent across the API.

## Evaluation Perspective

When evaluating AI-generated API guidance, I assess technical accuracy, completeness, practical usefulness, consistency, security awareness, and whether recommendations are appropriately qualified.
