# Lokal.ind API

This is an Node.js application that serves as an API for Lokal.ind, an online platform where you can shop for local fashion items. It includes various routes for managing brands, categories, products, orders, and more. This API is deployed by Google Cloud App Engine, PostgreSQL on CloudSQL for relational database and Cloud Storage Bucket for storing images.

## Features

- RESTful API endpoints for:
  - Brands
  - Categories
  - Products
  - Shippers
  - Payments
  - Order Status
  - Authentication
  - Cart
  - Wishlist
  - Orders
  - Recommendations
- Swagger UI for API documentation
- CORS support
- Error handling

## Get Started

1. Clone repository with command `git clone <repo_url>`
2. Move to directory `cd Cloud-Computing-API`
3. Fill the .env file with your own configuration

> Local Configuration
5. Install dependencies using command `npm install`
6. Running the server `npm run dev`.

**or**

> Google Cloud Deployment
5. Create `app.yaml` file in the root directory and rename the service name  
```
runtime: nodejs18  
service: Your_Service_Name
```
6. Deploy to app.engine with command `gcloud app deploy`.

## Google Cloud Infrastructure
![Infrastucture Image](Infrastucture/Lokal.ind%20Diagram.png)

## API Documentation

Access the Swagger UI of Lokal.ind API documentation at [Loakl.ind Swagger UI](https://lokal-ind.et.r.appspot.com/api-docs).
> The Authorization was created manually using JWT(JSON Web Tokens).

## Routes

- `/brands`: Brand-related operations
- `/categories`: Category-related operations
- `/products`: Product-related operations
- `/shippers`: Shipper-related operations
- `/payments`: Payment-related operations
- `/orderStatus`: Order status operations
- `/auth`: Authentication routes
- `/cart`: Shopping cart operations
- `/wishlist`: Wishlist operations
- `/orders`: Order management
- `/recommendation`: Product recommendations

## Error Handling

The application boasts advanced custom error handling mechanisms designed to gracefully manage occurrences such as 404 Not Found and other potential errors with precision and efficiency

