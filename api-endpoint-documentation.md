# API Endpoint Documentation
## Get User
Retrieves information about a specific user
### Endpoint
**Method:** `GET`
**URL:** `/users/{user_id}`
Example 
/User/123
### Path Parameters
| Parameter | Type | Description |
|-----------|------|-------------|
| user_id | integer | The unique ID of the user. |
### Response 
Returns the details of the requested user.
#### Success Response
**Status Code** `200 ok`
```json
{
    "id": 123
    "name": "John Doe"
    "email": "john@example.com"
}
```
## Error Responses 
#### 404 Not Found 
The requested user does not exist.
#### 400 Bad Request
The user ID provided is invalid.