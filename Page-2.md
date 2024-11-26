# Authentication

## Getting Started
To authenticate with the API, you'll need an API key. You can obtain one from the developer dashboard.

### API Key Usage
Include your API key in the request header:

```http
Authorization: Bearer your-api-key-here
```

### Token Expiration
- Access tokens expire after 24 hours
- Refresh tokens expire after 30 days

## Security Best Practices
1. Never share your API keys
2. Rotate keys regularly
3. Use environment variables to store keys
4. Implement key rotation procedures