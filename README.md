# 🎓 University Management System

## Overview

**University Management System** is a web-based application designed to automate and simplify core academic processes within a university environment.

The system provides role-based access for **Students** and **Teachers**, ensuring structured interaction, secure authentication, and efficient academic management.

This project was developed using **Java Spring Framework** as part of the **End-term Defense for the Software Design Patterns (SDP)** course at **Astana IT University**.

---

## 🚀 Key Features

### 🔐 Authentication & Authorization

* Secure login and registration
* JWT-based authentication
* Role-based access control (Student / Teacher)
* Spring Security integration

### 👨‍🎓 Student Dashboard

* View assigned group
* View enrolled courses
* View teachers associated with courses
* Read-only structured academic information

### 👨‍🏫 Teacher Dashboard

* View assigned groups
* Manage student lists
* Edit group composition
* Structured group management interface

### 🏗 Architecture

* Layered architecture (Controller → Service → Repository)
* Clean separation of concerns
* RESTful API design principles
* Scalable and maintainable backend structure

---

## 🛠 Tech Stack

### Backend

* Java 17+
* Spring Boot
* Spring Security
* Spring Data JPA
* Hibernate

### Database

* PostgreSQL

### Authentication

* JSON Web Tokens (JWT)

### Frontend

* HTML
* CSS

---

## 📂 Project Structure

```
src/
 ├── controller/
 ├── service/
 ├── repository/
 ├── entity/
 ├── config/
 └── dto/
```

* **controller** — REST endpoints
* **service** — business logic
* **repository** — database interaction
* **entity** — JPA entities
* **config** — security & application configuration
* **dto** — data transfer objects

---

## ⚙️ How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/university-management-system.git
cd university-management-system
```

### 2️⃣ Configure Database

Update `application.yml` or `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/university_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

Make sure PostgreSQL is running.

### 3️⃣ Run the Application

Using Maven:

```bash
mvn spring-boot:run
```

Or:

```bash
./mvnw spring-boot:run
```

Application will start at:

```
http://localhost:8080
```

---

## 🔐 Security Implementation

* Stateless authentication
* JWT access token validation
* Custom UserDetails implementation
* Password hashing with BCrypt
* Protected endpoints based on roles

---

## 📌 Design Patterns Applied

This project demonstrates practical implementation of:

* **Singleton** (Spring Beans)
* **Factory Method** (Bean creation & configuration)
* **Dependency Injection**
* **Repository Pattern**
* **DTO Pattern**
* **Layered Architecture Pattern**

---

## 🎯 Educational Purpose

This system was built to:

* Practice Software Design Patterns
* Implement secure authentication with Spring Security
* Design a clean and maintainable backend architecture
* Work with relational databases using JPA
* Develop a role-based web application

---

## 📄 License

This project was developed for academic purposes.
