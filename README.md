# User Management REST API with JWT Authentication

This is a Spring Boot-based REST API for user management, including features like registration, login, JWT-based authentication, and role-based authorization (ROLE_USER, ROLE_ADMIN).

---

## 📌 Features

- ✅ User Registration
- ✅ User Login with JWT Token Generation
- ✅ JWT Token Validation on Secure Endpoints
- ✅ Role-based Access Control (`ROLE_USER`, `ROLE_ADMIN`)
- ✅ Password encryption using BCrypt
- ✅ Global Exception Handling
- ✅ Spring Security Integration

---

## 🧱 Technologies Used

- Java 17
- Spring Boot
- Spring Security
- JWT (JSON Web Token)
- MySQL
- JPA / Hibernate
- Maven

---

## 🔧 API Endpoints

### 🔐 Authentication APIs

| Method | Endpoint     | Description            |
|--------|--------------|------------------------|
| POST   | `/register`  | Register a new user    |
| POST   | `/login`     | Login and get JWT token|

### 👤 User APIs (Secured with JWT)

| Method | Endpoint        | Role Required |
|--------|------------------|----------------|
| GET    | `/users`         | ROLE_ADMIN     |
| GET    | `/users/{id}`    | ROLE_USER/ADMIN|
| DELETE | `/users/{id}`    | ROLE_ADMIN     |

---

## 🗂️ Project Structure

