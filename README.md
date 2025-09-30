Here’s the **complete and cleaned-up `README.md` content** for your Shopping Cart Application. You can copy and paste this directly into your project:

# 🛒 Shopping Cart Application

## 📚 Table of Contents
- Overview
- Technical Stack
- Setup and Installation
- API Documentation
- Cart Operations
- Configuration Guide

---

## 🧾 Overview
A robust shopping cart application built using **Spring Boot**, designed to manage product listings, user carts, and checkout functionality. It includes RESTful APIs and an in-memory database for quick setup and testing.

---

## 🛠️ Technical Stack
- Java 11  
- Spring Boot 2.7.8  
- Spring MVC  
- Spring Data JPA  
- Maven  
- H2 In-Memory Database  

---

## ⚙️ Setup and Installation

### ✅ Prerequisites
- JDK 11  
- Maven 3.6+  

### 🚀 Build and Run

bash
mvn clean install
java -jar target/shopping-cart-test-java-1.0.0.jar


### 🌱 Environment
- Uses **H2 in-memory database**
- Preloaded with sample data via SQL script

---

## 📘 API Documentation

### 🔗 Swagger UI
Access the Swagger UI at:  
http://localhost:8080/swagger-ui/

### 📦 Create Product

**Endpoint:** `POST /api/products`  
**Content-Type:** `application/json`

**Sample Request Body:**
{
  "name": "Product Name",
  "description": "Product Description",
  "price": 99.99,
  "category": "ELECTRONICS",
  "stockQuantity": 100
}


---

## 🛒 Cart Operations

### Controllers Overview

#### 1. `CartController`
- Add product to cart
- Get cart by `userId`
- Remove product from cart
- Checkout cart

#### 2. `ProductController`
- Add new product
- Get all available products

#### 3. `UserController`
- Add new user

---

## ⚙️ Configuration Guide
- All configurations are handled via `application.properties`
- H2 console available at: http://localhost:8080/h2-console
