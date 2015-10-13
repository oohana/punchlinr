Punchlinr
=========

API
---

### Authentication

* `POST /auth`

This endpoint provides three different ways to authenticate users:
- User Credentials
- JSON Web Tokens (JWT)
- Facebook Access Tokens

JWT should be stored client-side on local storage

```javascript
POST /auth
Content-Type: application/json

{
  "username": "username",
  "password": "password"
}
---
HTTP/1.1 201 Created
Content-Type: application/json

{
    "item": {
        "created": "2015-02-20T02:06:35.378992304-08:00",
        "id": "54e7072ba6ebe4f02b000001",
        "name": "Account Name",
        "service": "<service>"
    },
    "status": "OK"
}
```
