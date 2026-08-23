# User API Documentation
## Overview
This API allows developers to retrieve information about a user.
## Get User
Retrieve information about a specific user.
### Endpoint 
`GET/api/users/{id}`
### Path Parameter
| Parameter | Type | Required | Description |
|-----------|------|----------|-------------|
| id | integer | Yes | The unique ID of the user.|
### Request Example 
```http
GET /api/users/123
```
### Response Example 
```json
{
    "id": 123
    "name": "John Doe"
    "email": "john@example.com"
}
```
## Error Responses
### 404 Not Found
The requested user does not exist.
### 400 Bad Request
The user ID provided is invalid.
