# API Documentation Basics
## Overview
This document introduces the basic structure of API documentation.
## What is an API
An API (Application Programming Interface) allows different software application to communicate with each other.
## Example Endpoint
**GET** `/users`
### Description
Returns a list of users.
### Request
```http
GET /users HTTP/1.1
Host: example.com
```
### Response
```json
[ 
     { "id": 1,
       "name": "John Doe"
     }
]
```
## Status Codes
| Code | Meaning |
|------|---------|
| 200 | Request successful |
| 404 | Resource not found |
| 500 | Internal server error |
## Conclusion 
Good API documentation helps developers understand and use API correctly.
## Tips
- Use clear and simple language.
- Include request and response example.
- Explain status codes.
- Keep the documentation up to date.
