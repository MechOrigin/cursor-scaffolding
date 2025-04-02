# API Documentation

## Overview

This document outlines the API structure and guidelines for the backend services.

## API Guidelines

### RESTful Conventions

- Use HTTP methods appropriately:
  - GET: Retrieve resources
  - POST: Create resources
  - PUT: Update entire resources
  - PATCH: Partial updates
  - DELETE: Remove resources

### Response Format

```typescript
interface ApiResponse<T> {
  success: boolean;
  data?: T;
  error?: {
    code: string;
    message: string;
    details?: unknown;
  };
  meta?: {
    page?: number;
    limit?: number;
    total?: number;
  };
}
```

### Error Handling

- Use appropriate HTTP status codes:
  - 200: Success
  - 201: Created
  - 400: Bad Request
  - 401: Unauthorized
  - 403: Forbidden
  - 404: Not Found
  - 500: Internal Server Error

### Authentication

- JWT-based authentication
- Include token in Authorization header:
  ```
  Authorization: Bearer <token>
  ```

## API Endpoints

### Authentication

```typescript
POST /api/auth/login
POST /api/auth/register
POST /api/auth/refresh-token
POST /api/auth/logout
```

### Users

```typescript
GET /api/users
GET /api/users/:id
PUT /api/users/:id
DELETE /api/users/:id
```

### Health Check

```typescript
GET /api/health
```

## Rate Limiting

- 100 requests per minute per IP
- 1000 requests per hour per user

## API Versioning

- Current version: v1
- Include version in URL: `/api/v1/...`

## OpenAPI/Swagger

API documentation is available at `/api-docs` when running in development mode. 