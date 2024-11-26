# Error Handling

## HTTP Status Codes
Our API uses standard HTTP status codes to indicate the success or failure of requests.

- 200: Success
- 201: Created
- 400: Bad Request
- 401: Unauthorized
- 403: Forbidden
- 404: Not Found
- 429: Too Many Requests
- 500: Internal Server Error

## Error Response Format
```json
{
    "error": {
        "code": "INVALID_PARAMETER",
        "message": "The provided parameter is invalid",
        "details": {
            "field": "email",
            "reason": "Invalid email format"
        }
    }
}
```