# API Authentication
## Overview 
API authentication is the process of verifying that a user or application is allowed to access an API.
This guide explains how to authenticate requests using an API key and a bearer token.
## API Key Authentication 
An API key is a unique value used to identify an application when making API request header.
Include the API key in the request header.
### Request Header 
```text
x-API-key: YOUR_API_KEY
```
### Example Request
```bash
curl https://api.example.com/users \
-H "X-API-key: YOUR_API_KEY"
```
```markdown
## Bearer Token Authentication
A bearer token is a security credential that allows an authenticated application to access an API.
Include the token in the `Authorization` header.
### Request Header 
```text
Authorization: Bearer YOUR_ACCESS_TOKEN
```
### Example Request
```bash
curl https://api.example.com/users \
-H "Authorization: Bearer YOUR_ACCESS_TOKEN"
```
## Security Best Practices
- Never share your API keys or access tokens publicly.
- Store sensitive credentials in environment variables.
- Do not commit API keys or tokens to GitHub.
- Use HTTPS to protect credentials while they are being transmitted.
- Rotate API keys regularly when necessary.
## Conclusion
API authentication helps protect APIs by ensuring that only authorised users and applications can access protected resources.
API keys and bearer tokens are common authentication methods, but they should always be handled securely.