# 🎓 Student Management System

A **Spring Boot REST API** for managing student records with **MySQL** database integration. This project implements full **CRUD operations** following industry-standard **3-layered architecture**.

---

## 🎯 Overview

This project is a backend REST API service that allows users to perform CRUD operations (Create, Read, Update, Delete) on student records. It demonstrates core concepts of:

- Spring Boot framework
- RESTful API design
- JPA & Hibernate ORM
- MySQL database integration
- Layered architecture (Controller → Service → Repository)
- Dependency Injection
- HTTP methods and status codes

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| **Language** | Java 17 |
| **Framework** | Spring Boot 4.0.6 |
| **ORM** | Spring Data JPA + Hibernate |
| **Database** | MySQL 9.7 |
| **Build Tool** | Maven |
| **IDE** | IntelliJ IDEA |
| **Testing Tool** | Postman |

---

## 🏗️ Architecture

This project follows the standard **3-Layered Architecture**:

- **Controller Layer** (`@RestController`) — Handles HTTP requests and responses
- **Service Layer** (`@Service`) — Contains business logic
- **Repository Layer** (`@Repository`) — Manages database operations using JpaRepository
- **Entity Layer** (`@Entity`) — Maps Java objects to MySQL tables

---

## ✨ Features

- ➕ Create new student records
- 📖 Read all students or a specific student by ID
- ✏️ Update existing student information
- 🗑️ Delete student records
- 🔐 Unique email validation
- 🆔 Auto-generated student IDs

---

## 🌐 API Endpoints

| Method | Endpoint | Description | Status Code |
|--------|----------|-------------|-------------|
| `POST` | `/api/students` | Create a new student | 201 Created |
| `GET` | `/api/students` | Get all students | 200 OK |
| `GET` | `/api/students/{id}` | Get a student by ID | 200 OK |
| `PUT` | `/api/students/{id}` | Update a student | 200 OK |
| `DELETE` | `/api/students/{id}` | Delete a student | 200 OK |

---

## ⚙️ Setup Instructions

### Prerequisites

- Java 17 or higher
- Maven 3.8+
- MySQL 8.0+
- IntelliJ IDEA (recommended)

### Step 1: Clone the Repository
git clone https://github.com/Fasttyper1/student-management-system-.git
cd student-management-system-

### Step 2: Create MySQL Database
CREATE DATABASE studentdb;

### Step 3: Configure Database
Update `src/main/resources/application.properties`:

### Step 4: Run the Application
Application starts at `http://localhost:8080`

---

## 📬 Sample API Requests

### Create Student (POST)

**Request:**
**Response (200 OK):**
### Update Student (PUT)# 🎓 Student Management System

A **Spring Boot REST API** for managing student records with **MySQL** database integration. This project implements full **CRUD operations** following industry-standard **3-layered architecture**.

## 🎯 Overview

This project is a backend REST API service that allows users to perform CRUD operations (Create, Read, Update, Delete) on student records. It demonstrates core concepts of:

- Spring Boot framework
- RESTful API design
- JPA & Hibernate ORM
- MySQL database integration
- Layered architecture (Controller → Service → Repository)
- Dependency Injection
- HTTP methods and status codes

## 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Language | Java 17 |
| Framework | Spring Boot 4.0.6 |
| ORM | Spring Data JPA + Hibernate |
| Database | MySQL 9.7 |
| Build Tool | Maven |
| IDE | IntelliJ IDEA |
| Testing Tool | Postman |

## 🏗️ Architecture

This project follows the standard 3-Layered Architecture:

- **Controller Layer** - Handles HTTP requests and responses
- **Service Layer** - Contains business logic
- **Repository Layer** - Manages database operations
- **Entity Layer** - Maps Java objects to MySQL tables

## ✨ Features

- Create new student records
- Read all students or a specific student by ID
- Update existing student information
- Delete student records
- Unique email validation
- Auto-generated student IDs

## 🌐 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/students | Create a new student |
| GET | /api/students | Get all students |
| GET | /api/students/{id} | Get a student by ID |
| PUT | /api/students/{id} | Update a student |
| DELETE | /api/students/{id} | Delete a student |

## ⚙️ Setup Instructions

### Prerequisites

- Java 17 or higher
- Maven 3.8+
- MySQL 8.0+

### Step 1: Clone the Repository

```
git clone https://github.com/Fasttyper1/student-management-system-.git
```

### Step 2: Create MySQL Database

```
CREATE DATABASE studentdb;
```

### Step 3: Configure Database

Update src/main/resources/application.properties:

```
spring.datasource.url=jdbc:mysql://localhost:3306/studentdb
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update
```

### Step 4: Run the Application

```
mvn spring-boot:run
```

Application starts at http://localhost:8080

## 📬 Sample API Request

### Create Student (POST)

Request:
```
POST http://localhost:8080/api/students
Content-Type: application/json

{
    "name": "Abhiram Vemuri",
    "email": "abhiram@gmail.com"
}
```

Response:
```
{
    "id": 1,
    "name": "Abhiram Vemuri",
    "email": "abhiram@gmail.com"
}
```

## 🚀 Future Enhancements

- Add input validation with @Valid
- Implement global exception handling
- Add Swagger documentation
- Integrate Spring Security with JWT
- Add pagination and sorting
- Add unit tests with JUnit
- Deploy to AWS/Heroku
- Add a React frontend

## 👤 Author

**Abhiram Vemuri**
- GitHub: [@Fasttyper1](https://github.com/Fasttyper1)
- Email: vemuriabhiram2005@gmail.com

⭐ If you found this project helpful, please give it a star! ⭐
**Request:**




