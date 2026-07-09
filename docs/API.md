# API Documentation

## Authentication

All API requests require a Bearer token in the Authorization header.

## Endpoints

### Products
- `GET /api/products` - List all products
- `POST /api/products` - Create new product
- `GET /api/products/:id` - Get product details
- `PUT /api/products/:id` - Update product
- `DELETE /api/products/:id` - Delete product

### Inventory
- `GET /api/inventory` - Current stock levels
- `POST /api/inventory/adjust` - Adjust stock
- `GET /api/inventory/low` - Low stock alerts
