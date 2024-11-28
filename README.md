Role-Based Access Control (RBAC) System

Project Overview

This project is a Role-Based Access Control (RBAC) system implemented in Java using Spring Boot. It includes features like secure user authentication, role-based authorization, and protected endpoints accessible only to users with the appropriate roles. The system ensures that users can only access resources and perform actions based on their assigned roles.

Features

User Authentication: Secure login and logout using JWT (JSON Web Tokens).
Role-Based Authorization: Access control based on user roles (e.g., Admin, User, Moderator).
Protected Endpoints: Resources restricted to specific roles.
Secure Password Management: Passwords are hashed using BCrypt.
Custom Role Hierarchy: Easy to manage and extend user roles and permissions.

Technologies Used
Java 17
Spring Boot
Spring Security
Spring Data JPA
JWT (JSON Web Tokens)
MYSQL (for development and testing)
Postman (for API testing)


Endpoints
Authentication

Register: POST /api/auth/register
Login: POST /api/auth/login


Testing with Postman

Register a new user (/api/auth/register).
Log in to obtain a JWT (/api/auth/login).
Add the JWT to the Authorization Header:
Authorization: Bearer <jwt_token>
Access the protected endpoints (e.g., /api/admin/dashboard).


Security Best Practices

Passwords are hashed using BCrypt for secure storage.
Tokens are validated before granting access to protected resources.
Spring Security ensures role-based access to endpoints.

Future Enhancements

Add support for OAuth2-based authentication.
Implement refresh tokens for token expiration handling.
Integrate with an external database like MySQL.

