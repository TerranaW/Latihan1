# Authentication

## Register

- **Endpoint**: `POST /auth/register`
- **Description**: Register user baru.

  ### Request Body :
```json
{
  "username": "example",
  "email": "example@example.com",
  "password": "password123"
}

  ### Response Body:
- Status Code : 201
```json
{
  message : "sucessfully registered"
}
