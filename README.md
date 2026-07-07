# 🏦 Banking Management System

A backend Banking Management System developed using **Java**, **Spring Boot**, **Spring MVC**, **Spring Data JPA**, **Hibernate**, and **MySQL**. The application exposes RESTful APIs for managing bank accounts and follows a clean layered architecture for scalability and maintainability.



## ✨ Features

- Create a new bank account
- Retrieve account details
- Update account information
- Delete a bank account
- Deposit money
- Withdraw money
- View all bank accounts
- RESTful API design
- Exception handling
- Layered architecture



## 🛠 Tech Stack

| Category | Technologies |
|----------|--------------|
| Language | Java |
| Framework | Spring Boot, Spring MVC |
| ORM | Spring Data JPA, Hibernate |
| Database | MySQL |
| Build Tool | Maven |
| API Testing | Postman |
| Version Control | Git & GitHub |



## 📁 Project Structure

```
src
├── controller
│   └── AccountController.java
├── service
│   ├── AccountService.java
│   └── impl
│       └── AccountServiceImpl.java
├── repository
│   └── AccountRepository.java
├── entity
│   └── Account.java
├── dto
│   └── AccountDto.java
├── entity
│   └── mapper
│       └── AccountMapper.java
└── BankingAppApplication.java
```



## 🏗 Architecture

```
Client
   │
REST API
   │
AccountController
   │
AccountService
   │
AccountRepository
   │
MySQL Database
```



## ⚙ Installation

### Clone the repository

```bash
git clone https://github.com/your-username/banking-app.git
```

### Navigate to the project

```bash
cd banking-app
```

### Configure MySQL

Update `application.properties`

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/banking_db
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```



## ▶ Running the Application

Using Maven

```bash
mvn spring-boot:run
```

Or run

```
BankingAppApplication.java
```

The application starts on

```
http://localhost:8080
```



## 📌 REST API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/accounts | Create Account |
| GET | /api/accounts/{id} | Get Account by ID |
| GET | /api/accounts | Get All Accounts |
| PUT | /api/accounts/{id} | Update Account |
| DELETE | /api/accounts/{id} | Delete Account |
| POST | /api/accounts/{id}/deposit | Deposit Money |
| POST | /api/accounts/{id}/withdraw | Withdraw Money |




## 🧪 API Testing

All APIs were tested using **Postman**.

Example Request

```http
POST /api/accounts/{id}/deposit
```

```json
{
    "amount": 5000
}
```

Example Response

```json
{
    "message": "Amount deposited successfully"
}
```



## 🎯 Concepts Used

- Java
- Spring Boot
- Spring MVC
- Spring Data JPA
- Hibernate
- REST APIs
- CRUD Operations
- DTO Pattern
- Entity Mapping
- Layered Architecture
- Dependency Injection
- Exception Handling



## 🚀 Future Enhancements

- JWT Authentication
- Spring Security
- Fund Transfer Module
- Transaction History
- Account Statements
- Unit Testing using JUnit & Mockito
- Docker Deployment
- React.js Frontend Integration



## 👩‍💻 Author

**Namrutha Srinidhi T**

- LinkedIn: https://www.linkedin.com/in/namrutha-srinidhi-t-746baa246
- GitHub: https://github.com/Namrutha20



⭐ If you found this project useful, consider giving it a star!
