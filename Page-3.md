# API Endpoints

## Users

### GET /api/v1/users
Retrieve a list of users.

**Parameters:**
- `page` (optional): Page number for pagination
- `limit` (optional): Number of items per page

**Response:**
```json
{
    "users": [
        {
            "id": 1,
            "name": "John Doe",
            "email": "john@example.com"
        }
    ],
    "total": 100,
    "page": 1
}
```

### POST /api/v1/users
Create a new user.

**Request Body:**
```json
{
    "name": "John Doe",
    "email": "john@example.com",
    "password": "securepassword"
}
```

## Products

### GET /api/v1/products
Retrieve a list of products.

### POST /api/v1/products
Create a new product.