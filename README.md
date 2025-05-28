## E-commerce API with Authentication

A RESTful API built with Node.js, Express, and MongoDB to manage users, products, and shopping carts. It allows users to register, login, and perform CRUD operations on products and carts with full authentication and authorization.

## Live Link: https://e-commerce-api-with-authentication-8ndm.onrender.com

⸻

## Features
-	🔐 User registration and login with secure password hashing.
-	🛒 JWT-based authentication and authorization to protect endpoints.
-	📦 Create, read, update, and delete products.
-	🛍️ Add, remove, clear, and update product quantities in user carts.
-	🛠️ Input validation and robust error handling (can be added).
-	🔄 Modular and scalable backend architecture.

⸻

## Technologies Used
-	**Node.js** — JavaScript runtime environment.
-	**Express** — Web framework for Node.js.
-	**MongoDB** — NoSQL database for storing users, products, and carts.
-	**Mongoose** — ODM for MongoDB schema modeling.
-	**bcryptjs** — Password hashing for user security.
-	**jsonwebtoken**— JWT creation and verification for authentication.
-	**dotenv** — Environment variable management.
-	**cors** — Middleware for Cross-Origin Resource Sharing.

⸻

## API Endpoints Overview
### User API Endpoints

| Method | Endpoint           | Description            | Auth Required |
|--------|--------------------|------------------------|---------------|
| POST   | /api/user/register | Register a new user    | No            |
| POST   | /api/user/login    | Login and get JWT token | No            |

---

### Product API Endpoints

| Method | Endpoint           | Description              | Auth Required |
|--------|--------------------|--------------------------|---------------|
| POST   | /api/product/add   | Add a new product        | Yes           |
| GET    | /api/product/all   | Get all products         | No            |
| GET    | /api/product/:id   | Get product by ID        | No            |
| PUT    | /api/product/:id   | Update product by ID     | Yes           |
| DELETE | /api/product/:id   | Delete product by ID     | Yes           |

---

### Cart API Endpoints

| Method | Endpoint                   | Description                         | Auth Required |
|--------|----------------------------|-----------------------------------|---------------|
| POST   | /api/cart/add              | Add product to cart                | Yes           |
| GET    | /api/cart/user             | Get current user's cart            | Yes           |
| DELETE | /api/cart/remove/:productId| Remove product from cart           | Yes           |
| DELETE | /api/cart/clear            | Clear the entire cart              | Yes           |
| POST   | /api/cart/--qty            | Decrease product quantity in cart | Yes           |


## Testing
- Use tools like Postman or Thunder Client to test the API endpoints.
- Include the JWT token in the Auth header for protected routes in this format:

⸻

## Screenshots

⸻

## Demo Video

⸻
