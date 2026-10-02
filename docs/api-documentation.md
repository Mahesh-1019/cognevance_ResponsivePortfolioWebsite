# REST API Documentation

Base URL: `http://localhost:5000`

## GET /api/health
Returns API health status.

Example response:
```json
{ "status": "ok", "service": "portfolio-api" }
```

## POST /api/contact
Stores a contact form message.

Request:
```json
{
  "name": "Alex",
  "email": "alex@example.com",
  "message": "Hello, I would like to connect."
}
```

Success:
```json
{
  "message": "Contact message saved.",
  "id": "..."
}
```

Validation errors return HTTP 400. Database/server failures return HTTP 500.

## GET /api/contact
Returns the latest saved contact messages. This endpoint is intended for development/demo verification and should be protected with authentication before production use.
