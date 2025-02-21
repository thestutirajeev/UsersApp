# 🚀 User REST API - Spring Boot

## 🌟 Overview
This project is a RESTful API for managing users, built using Spring Boot. It provides endpoints to create, retrieve, update, and delete user records.

## 🛠️ Tech Stack
- ⚡ **Spring Boot 3.4.3**
- 🌍 **Spring Boot Starter Web** (for building REST APIs)
- 💾 **Spring Boot Starter Data JPA** (for database interaction)
- 🛢️ **MySQL** (for persistent storage)
- 🔄 **Spring Boot DevTools** (for development efficiency)
- ✅ **Spring Boot Starter Test** (for testing)

## 🎯 Features
- ➕ Create a new user
- 📜 Retrieve all users
- 🔍 Retrieve a specific user by ID
- ✏️ Update an existing user
- ❌ Delete a user

## 📌 API Endpoints
| 🏷️ HTTP Method | 🔗 Endpoint | 📄 Description |
|------------|----------------|-------------|
| 📝 POST | `/api/users` | Create a new user |
| 📥 GET | `/api/users` | Retrieve all users |
| 🔎 GET | `/api/users/{id}` | Retrieve a user by ID |
| 🛠️ PUT | `/api/users/{id}` | Update an existing user |
| 🗑️ DELETE | `/api/users/{id}` | Delete a user |

## ⚙️ Setup and Installation
### 📌 Prerequisites
- ☕ Java 22
- 🏗️ Maven
- 🛢️ MySQL database

### 🚀 Steps to Run
1. **Clone the repository:**
2. **Configure MySQL Database:**
   - Open `application.properties` (or `application.yml` if you use YAML) and configure your database settings:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     spring.jpa.hibernate.ddl-auto=update
     ```
3. **Build and Run the Project:**
   ```sh
   mvn spring-boot:run
   ```
4. **Test the API:**
   - Use 🛠️ **Postman** to test the API endpoints by sending requests and verifying responses.
   - Alternatively, use `curl` commands in the terminal.

## 📌 Prerequisites
- **Java 17+**
- **Spring Boot 3+**
- **MySQL Server**
- **Postman** (for testing API)

## 🏗️ Project Structure
```
User_Rest_SpringBoot
│── src/main/java/com/example/demo
│   ├── controller/UserController.java
│   ├── model/User.java
│   ├── repository/UserRepository.java
│   ├── service/UserService.java
│   └── DemoApplication.java
│── src/main/resources/
│   ├── application.properties
│── pom.xml
```

## 📜 License
This project is licensed under the MIT License. 📄
