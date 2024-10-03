### Amazon E-commerce Back-end Project

This project, developed by Dandamoodi Bharath, implements the back-end services for an Amazon-like e-commerce platform. The primary focus of the project is on building robust, scalable, and efficient REST APIs that facilitate core operations of an e-commerce website, including user authentication, product management, order processing, and payment handling. The back-end is built using Java and incorporates several key frameworks and technologies to ensure seamless performance and reliability.

## Project Overview

Amazon is one of the largest e-commerce platforms globally, serving millions of users. This back-end project is designed to simulate the fundamental operations of such an e-commerce system, handling customer data validation, business logic processing, and persistent data storage in the database. The system allows for seamless CRUD operations on entities like users, products, orders, and payments.

The business logic ensures that only valid and authorized requests are processed, such as validating user credentials during login, checking stock availability before processing an order, and calculating total prices with applicable discounts and taxes.

## Key Features

- **User Management**: 
  - Registration and login functionality with JWT-based authentication.
  - User roles and authorization to control access to certain resources.
  
- **Product Management**:
  - CRUD operations for product catalog with search and filter functionalities.
  - Business logic to handle stock management and real-time updates on product availability.

- **Order Management**:
  - Placing, tracking, and managing orders.
  - Validations for payment and order status updates.

- **Payment Integration**:
  - Handling various payment gateways and processing payment status.
  - Secure transactions using encryption and validation layers.

- **Shopping Cart**: 
  - Add/remove products, calculate total price, and manage cart items.
  - Business logic for promotions, discounts, and taxes.

## Technologies and Tools Used

- **Java**: Core programming language for writing the back-end logic.
- **Spring Boot**: To create a stand-alone, production-ready Spring-based application with ease.
- **Spring Data JPA**: For seamless integration with the database and handling of complex queries.
- **Hibernate**: ORM framework to map Java objects to relational database tables, ensuring efficient data handling.
- **MySQL**: The relational database used to store and manage all the application’s data.
- **Spring Security**: For implementing authentication and role-based authorization, securing the APIs.
- **RESTful APIs**: For building the web services that interact with the front-end and other third-party services.
- **Maven**: For dependency management and project build automation.

## Database Schema

The database is structured with normalized tables representing core entities such as:
- **Users**: Stores user details, roles, and credentials.
- **Products**: Contains details about products, stock, and pricing.
- **Orders**: Keeps track of all user orders, including order status, payment details, and delivery tracking.
- **Payments**: Manages payment status, transaction history, and payment gateway interactions.

## API Documentation

Each endpoint follows REST principles and is structured as follows:
- **POST /api/users/register**: Register a new user.
- **POST /api/users/login**: Authenticate a user and issue a JWT token.
- **GET /api/products/{id}**: Retrieve product details by product ID.
- **POST /api/orders**: Create a new order.
- **PATCH /api/orders/{id}/status**: Update order status (e.g., shipped, delivered).
- **POST /api/payments/process**: Process a payment for an order.

---

This project highlights the use of Spring's powerful ecosystem, best practices in back-end development, and a deep understanding of how e-commerce platforms handle business operations at scale.
