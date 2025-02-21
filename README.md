# Users REST API - Spring Boot

This is a simple **Users REST API** built with **Spring Boot** to demonstrate basic CRUD operations. The API interacts with a MySQL database to manage user data.

## 🛠 Tech Stack
- **Spring Boot** (Spring MVC, Spring Data JPA)
- **Hibernate**
- **MySQL**
- **HikariCP** (Connection Pooling)
- **Postman** (For API Testing)

## 📂 Project Structure
```
src/main/java/com/example/demo/
│── controller/     # Handles API requests
│── service/        # Business logic layer
│── repository/     # Data access layer
│── model/          # User entity definition
│── config/         # Database and application configuration
│── DemoApplication # Main Spring Boot application
```

## 📌 Prerequisites
- **Java 17+**
- **Spring Boot 3+**
- **MySQL Server**
- **Postman** (for testing API)

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/users-rest-api.git
cd users-rest-api
```

### 2️⃣ Configure MySQL Database  
Create a database in MySQL:
```sql
CREATE DATABASE usersdb;
```
Update `application.properties` (or `application.yml`) in `src/main/resources`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/usersdb
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
```

### 3️⃣ Build and Run the Application
```sh
mvn clean install
mvn spring-boot:run
```

## 📌 API Endpoints for Postman Testing

| Method | Endpoint        | Description           |
|--------|----------------|-----------------------|
| GET    | `/api/users`   | Fetch all users      |
| GET    | `/api/users/{id}` | Fetch user by ID  |
| POST   | `/api/users`   | Create a new user    |
| PUT    | `/api/users/{id}` | Update user by ID |
| DELETE | `/api/users/{id}` | Delete user by ID |
