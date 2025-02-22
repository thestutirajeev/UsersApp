# 🚀 User REST API - Spring Boot  

## 🌟 Overview  
This project is a RESTful API for managing users, built using Spring Boot. It provides endpoints to create, retrieve, update, and delete user records. Additionally, a **frontend using Fetch API** is implemented to interact with the backend.  

## 🛠️ Tech Stack  
- ⚡ **Spring Boot 3.4.3**  
- 🌍 **Spring Boot Starter Web** (for building REST APIs)  
- 💾 **Spring Boot Starter Data JPA** (for database interaction)  
- 🛢️ **MySQL** (for persistent storage)  
- 🔄 **Spring Boot DevTools** (for development efficiency)  
- ✅ **Spring Boot Starter Test** (for testing)  
- 🖥️ **Fetch API (JavaScript)** (for frontend communication)  

## 🎯 Features  
- ➕ Create a new user  
- 📜 Retrieve all users  
- 🔍 Retrieve a specific user by ID  
- ✏️ Update an existing user  
- ❌ Delete a user  
- 🌐 **Frontend UI with Fetch API** to interact with the REST API  

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

## 🏗️ Project Structure  
```
User_Rest_SpringBoot
│── src/main/java/com/example/demo
│   ├── controller/UserController.java
│   ├── model/User.java
│   ├── repository/UserRepository.java
│   ├── service/UserService.java
│   ├── exceptions/
│   ├── service/GlobalExceptionHandler.java
│   └── DemoApplication.java
│── src/main/resources/
│   ├── application.properties
│── src/main/webapp/
│   ├── index.html
│   ├── add.html
│   ├── delete.html
│   ├── update.html
│   ├── index.js
│   ├── add.js
│   ├── delete.js
│   ├── update.js
│── pom.xml
```  

## 🌐 Fetch API Implementation  
The frontend uses **Fetch API** to connect with the REST API:  

- **`index.js`** → Fetches and displays all users  
- **`add.js`** → Sends a `POST` request to add a user  
- **`delete.js`** → Sends a `DELETE` request and shows success/failure messages  
- **`update.js`** → Sends a `PUT` request to update user details  

