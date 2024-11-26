# Rate Limiting

## Limits
- Free tier: 100 requests per hour
- Pro tier: 1000 requests per hour
- Enterprise tier: Custom limits

## Headers
Rate limit information is included in the response headers:
```
X-RateLimit-Limit: 100
X-RateLimit-Remaining: 95
X-RateLimit-Reset: 1635724800
```

## Handling Rate Limits
When you exceed your rate limit:
1. You'll receive a 429 Too Many Requests response
2. The response will include a Retry-After header
3. Wait for the specified time before retrying