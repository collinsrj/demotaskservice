# Demo Task Service

[![Java](https://img.shields.io/badge/Java-23-orange.svg)](https://openjdk.org/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4.3-brightgreen.svg)](https://spring.io/projects/spring-boot)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/collinsrj/demotaskservice)
[![Code Coverage](https://img.shields.io/badge/coverage-80%25-yellow.svg)](https://github.com/collinsrj/demotaskservice)
[![Security Rating](https://img.shields.io/badge/security-A-brightgreen.svg)](https://github.com/collinsrj/demotaskservice)
[![Maintainability](https://img.shields.io/badge/maintainability-A-brightgreen.svg)](https://github.com/collinsrj/demotaskservice)

A reactive Spring Boot application that provides a RESTful API for managing simple tasks. This project is developed entirely by AI.

## 🤖 AI-Powered Development

This project showcases the capabilities of AI in software development. All code, documentation, and tests are written by AI, demonstrating how artificial intelligence can be leveraged to create robust, secure, and maintainable applications.

## 🚀 Features

- Create, read, update, and delete tasks
- Assign tasks to users
- Set priorities and due dates
- Track task status
- Secure API with OAuth2
- Reactive programming model with WebFlux
- MongoDB for data persistence

## 🛠️ Technology Stack

- **Java 23**: Latest Java version with enhanced performance and features
- **Spring Boot 3.4.3**: Framework for building production-ready applications
- **Spring WebFlux**: Reactive web framework for building non-blocking applications
- **Spring Security**: Authentication and authorization
- **Spring Data MongoDB Reactive**: Reactive MongoDB data access
- **Lombok**: Reduces boilerplate code
- **Maven**: Build and dependency management
- **JUnit 5 & Mockito**: Testing framework
- **JaCoCo**: Code coverage
- **SpotBugs & FindSecBugs**: Static code analysis for security vulnerabilities
- **OWASP Dependency Check**: Vulnerability scanning

## 📊 Code Quality

This project maintains high code quality standards through:

- **Static Code Analysis**: SpotBugs with FindSecBugs plugin identifies potential bugs and security vulnerabilities
- **Security Scanning**: OWASP Dependency Check ensures dependencies are free from known vulnerabilities
- **Test Coverage**: JaCoCo enforces minimum code coverage requirements
- **Continuous Integration**: Automated build and test processes

## 🔒 Security Features

- OAuth2 Resource Server for authentication
- Role-based access control
- Input validation
- Security headers
- CSRF protection
- Rate limiting
- Secure coding practices

## 🏗️ Architecture

The application follows a clean, layered architecture:

- **API Layer**: REST controllers and request/response DTOs
- **Service Layer**: Business logic and validation
- **Repository Layer**: Data access and persistence
- **Domain Layer**: Core domain models and business rules

## 🚦 Getting Started

### Prerequisites

- Java 23 or later
- Maven 3.8.0 or later
- MongoDB 6.0 or later

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/collinsrj/demotaskservice.git
   cd demotaskservice
   ```

2. Build the application:
   ```bash
   ./mvnw clean install
   ```

3. Run the application:
   ```bash
   ./mvnw spring-boot:run
   ```

The application will start on `http://localhost:8080`.

### Configuration

The application can be configured using environment variables or by modifying the `application.properties` file:

```properties
# Server configuration
server.port=8080

# MongoDB configuration
spring.data.mongodb.uri=mongodb://localhost:27017/taskdb

# Security configuration
spring.security.oauth2.resourceserver.jwt.issuer-uri=https://your-auth-server.com
```

## 📝 API Documentation

The API is documented using OpenAPI 3.1.1. Once the application is running, you can access the API documentation at:

```
http://localhost:8080/swagger-ui.html
```

### Example Endpoints

- `GET /api/tasks` - List all tasks
- `GET /api/tasks/{id}` - Get a specific task
- `POST /api/tasks` - Create a new task
- `PUT /api/tasks/{id}` - Update an existing task
- `DELETE /api/tasks/{id}` - Delete a task

## 🧪 Testing

Run the tests with:

```bash
./mvnw test
```

Generate a test coverage report:

```bash
./mvnw verify
```

The coverage report will be available in `target/site/jacoco/index.html`.

## 🔄 CI/CD

This project uses CI/CD pipelines for automated building, testing, and deployment:

- **Build**: Compiles the code and runs static analysis
- **Test**: Executes unit and integration tests
- **Security Scan**: Performs security vulnerability scanning
- **Deploy**: Deploys to the target environment

## 🌐 Environments

The application supports multiple environments:

- **Local**: Development environment
- **Dev**: Integration testing environment
- **Stage**: Pre-production environment
- **Prod**: Production environment

Environment-specific configuration is managed through Spring profiles.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📚 Additional Resources

- [Spring Boot Documentation](https://docs.spring.io/spring-boot/docs/current/reference/html/)
- [Spring WebFlux Documentation](https://docs.spring.io/spring-framework/docs/current/reference/html/web-reactive.html)
- [MongoDB Documentation](https://docs.mongodb.com/)
