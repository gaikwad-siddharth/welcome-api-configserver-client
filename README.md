# Welcome API (Config Client)

A Spring Boot REST API that acts as a **Spring Cloud Config Client**. This application retrieves its configuration from a centralized **Spring Cloud Config Server**, allowing externalized and environment-specific configuration management.

---

## 🚀 Features

- Spring Boot REST API
- Spring Cloud Config Client
- Centralized configuration management
- Externalized properties from Config Server
- Easy integration with microservices architecture

---

## 🛠️ Tech Stack

- Java 17+
- Spring Boot
- Spring Cloud Config Client
- Maven

---

## 📁 Project Structure

```
src
├── main
│   ├── java
│   │   └── in.siddharth.rest
│   │       └── WelcomeRestController.java
│   └── resources
│       └── application.yml
└── test
```

---

## ⚙️ Configuration

The application fetches configuration from the Spring Cloud Config Server.

Example `application.yml`

```yaml
spring:
  application:
    name: WELCOME-API

  config:
    import: optional:configserver:http://localhost:8888
```

The Config Server provides the following property:

```properties
msg=Welcome to Spring Cloud Config Server
```

---

## 📷 Sample 

```
GET http://localhost:8080/welcome

## 📂 Related Projects

- Config Server
- Eureka Server
- API Gateway
- Admin Server

---

## 👨‍💻 Author

**Siddharth Gaikwad**
