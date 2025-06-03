# AUTHX – Secure Authentication System

**AUTHX** is a robust and scalable authentication platform built with Node.js, Express.js, and MongoDB. It provides a secure and efficient way to handle user signup, login, and access control through JWT-based authentication.

---

## 🚀 Key Features

### ✅ User Signup
- Secure account creation with email and password.
- Passwords are hashed using **bcrypt**.
- Input validation with **Joi** (e.g., valid email format, strong password).

### 🔐 User Login
- Secure login with credential verification.
- Issues a **JWT (JSON Web Token)** upon successful login.
- JWT is used to authenticate future requests (stateless session).

### 🔄 Token-Based Authentication
- Stateless authentication using JWT.
- Tokens are stored securely on the client side (e.g., HTTP-only cookies or `localStorage`).
- Protected routes require valid JWT.

### 🚪 User Logout
- Logout function invalidates tokens and ends the user session.

### 🌐 RESTful API Endpoints
- Designed with REST principles for scalability and clarity.
- Uses standard HTTP methods: `GET`, `POST`, `PUT`, `DELETE`.

### 🛡 Input Validation
- Validates and sanitizes request data with **Joi**.
- Protects against malformed data and injection attacks.

### ⚠️ Structured Error Handling
- Consistent error messages and HTTP status codes.
- Simplifies debugging and improves client-side integration.

---

## 🧰 Technologies Used

- **Node.js** – Runtime environment for server-side JavaScript.
- **Express.js** – Lightweight framework for building APIs.
- **MongoDB** – NoSQL database for secure data storage.
- **bcrypt** – For secure password hashing.
- **JWT (jsonwebtoken)** – Stateless authentication via token.
- **Joi** – Input validation schema.
- **Middleware** – For authentication, validation, and error handling.

---

## 🔒 Security Best Practices

- **Password Hashing**: Uses bcrypt to hash passwords, ensuring they are never stored in plain text.
- **JWT Authentication**: Stateless tokens prevent session hijacking and simplify session management.
- **HTTPS (in production)**: All data is transmitted securely over SSL.

---

## 📦 API Endpoints

| Method | Endpoint               | Description              |
|--------|------------------------|--------------------------|
| POST   | `/api/auth/signup`     | Register a new user      |
| POST   | `/api/auth/login`      | Login and receive token  |
| GET    | `/api/user/profile`    | Access user profile (Protected) |

---

## 👨‍💻 Author

Developed by [Karan Kashyap]

---

