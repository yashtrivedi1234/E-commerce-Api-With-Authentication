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
- Key: Authorization
-Value: Login Token ( You get when you successfully login )

⸻

## Screen Shots

⸻

### User API Endpoints

⸻

## Register a new user 
<img width="1470" alt="Screenshot 2025-05-29 at 12 22 20 AM" src="https://github.com/user-attachments/assets/1ec57a6b-ad82-4c5f-a23f-3a7b3a05c5be" />

⸻

## Login and get JWT token
<img width="1470" alt="Screenshot 2025-05-29 at 12 26 23 AM" src="https://github.com/user-attachments/assets/fdb91511-3ed7-45d9-960b-19187f28f9a4" />

⸻

### Product API Endpoints

⸻

## Add a new product 
<img width="1470" alt="Screenshot 2025-05-29 at 12 27 49 AM" src="https://github.com/user-attachments/assets/23168126-12ec-4a89-ab0b-053de8e0e3cf" />

⸻

## Get all products 
<img width="1470" alt="Screenshot 2025-05-29 at 12 31 52 AM" src="https://github.com/user-attachments/assets/3e5348d9-3e00-4972-94e1-c5ea0ef14d83" />

⸻

## Get product by ID 
<img width="1470" alt="Screenshot 2025-05-29 at 12 33 30 AM" src="https://github.com/user-attachments/assets/99bb00cc-ed07-45ec-b72e-32b2228a6509" />

⸻

## Update product by ID 
<img width="1470" alt="Screenshot 2025-05-29 at 12 35 21 AM" src="https://github.com/user-attachments/assets/908226b4-11c0-4084-a5a5-279714400715" />

⸻

## Delete product by ID
<img width="1470" alt="Screenshot 2025-05-29 at 12 36 31 AM" src="https://github.com/user-attachments/assets/1dbe3b8a-31d9-434c-b596-dfb7c842e6f0" />

⸻
