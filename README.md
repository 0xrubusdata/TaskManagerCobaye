# TaskManagerCobaye

## 📌 Project Overview
TaskManagerCobaye is a simple **Task Manager** designed to demonstrate how the same application can be implemented in multiple **programming languages** and **frameworks**. This repository serves as a reference for developers who want to compare different tech stacks and architectures.

## 🏗️ Tech Stacks
The project is implemented in the following **languages & frameworks**, each in its own branch:

- **(Django)**:

   Architecture: MVC (MVT).
   
   Best practices: DRY, KISS, automated testing.

- **Python (FastAPI)**:

   Architecture: Clean Architecture or Hexagonal.

   Best practices: SOLID, automated testing, asynchronism.

- **Java (Spring Boot)**:

   Architecture: Clean Architecture, Hexagonal, or Microservices.

   Best practices: SOLID, automated testing, Spring Cloud for microservices.

- **JavaScript/TypeScript (NestJS)**:

   Architecture: Clean Architecture or Microservices.

   Best practices: SOLID, automated testing, NestJS modules.

- **Kotlin (Ktor)**:

   Architecture: Clean Architecture or Hexagonal.

   Best practices: SOLID, automated testing, asynchronism.

- **Go (Fiber/Echo)**:

   Architecture: Clean Architecture.

   Best practices: KISS, automated testing, simplicity.

- **Rust (Actix/Axum)**:

   Architecture: Clean Architecture.

   Best practices: SOLID, automated testing, memory safety.

- **PHP (Laravel/Symfony)**:

   Architecture: MVC.

   Best practices: DRY, automated testing, Eloquent ORM (Laravel).

- **C# (.NET Core/ASP.NET)**:

   Architecture: MVC or Clean Architecture.

   Best practices: SOLID, automated testing, Entity Framework.

- **Scala (Play Framework)**:

   Architecture: MVC or Clean Architecture.

   Best practices: SOLID, automated testing, asynchronism.

- **Haskell (Servant)**:

   Architecture: Clean Architecture.

   Best practices: SOLID, automated testing, type-safety.

## 🔑 Modern architectures
### MVC (Model-View-Controller):

Usage: Ideal for fullstack applications (Django, Laravel, ASP.NET Core).

- **Frameworks**:

   Django: Naturally follows the MVT (Model-View-Template) pattern, a variant of MVC.

   Laravel: Uses MVC to separate the business logic (Model), the display (View) and the controller (Controller).

   ASP.NET Core: With Razor Pages or MVC, it follows the MVC pattern.

- **Best practices**:

   Keep the business logic in the Models.

   Use the Views only for the display.

   Controllers should be lightweight and contain only the routing logic.

### Clean Architecture:

Usage: Perfect for APIs and modular applications (FastAPI, Spring Boot, NestJS, Ktor).

- **Frameworks**:

   FastAPI : You can structure your project in layers (entities, use cases, interfaces).

   Spring Boot : Use packages to separate the layers (domain, application, infrastructure).

   NestJS : With its modules, services and controllers, it is easy to apply Clean Architecture.

   Ktor : You can organize your project in layers to separate the business logic from the technical details.

- **Best practices**:

   Separate responsibilities in layers (entities, use cases, interfaces).

   Inward-facing dependencies (core does not depend on technical details).

   Use interfaces to decouple components.

### Hexagonal Architecture (Ports and Adapters) :

Usage : Ideal for applications where business logic must be independent of technical details (Spring Boot, NestJS, Ktor).

- **Frameworks**:

   Spring Boot : Use interfaces to define ports and implementations to adapt them.

   NestJS: With its providers and modules, you can easily implement this architecture.

   Ktor: You can define ports for use cases and adapters for databases or external APIs.

- **Best practices**:

   Business logic is at the center, surrounded by ports and adapters.

   Technical details (database, external APIs) are adapters.

### Microservices :

Usage : If you want to split your application into several independent services (Spring Boot, FastAPI, NestJS).

- **Frameworks**:

   Spring Boot : Ideal for creating microservices with Spring Cloud.

   FastAPI : Lightweight and performant, perfect for microservices.

   NestJS : With its native support for microservices, it is an excellent choice.

- **Best practices**:

   Each service should have a unique responsibility.

   Use an API Gateway to handle incoming requests.

   Communicate between services via asynchronous messages (Kafka, RabbitMQ) or HTTP calls.

### Event-Driven Architecture :

Usage : For reactive and scalable applications (Spring Boot, NestJS, FastAPI).

- **Frameworks**:

   Spring Boot : With Spring Cloud Stream or Kafka.

   NestJS : Supports events and asynchronous messages.

   FastAPI: You can use libraries like Celery or RQ to handle events.

- **Best practices**:

   Use events to decouple components.

   Make sure events are idempotent (to avoid side effects).

   Best practices (SOLID, DRY, KISS, etc.)

### SOLID:

   Single Responsibility Principle: Each class or function should have a single responsibility.

   Open/Closed Principle: Components should be open to extension but closed to modification.

   Liskov Substitution Principle: Subclasses should be able to override their base classes.

   Interface Segregation Principle: Prefer specific interfaces over generic ones.

   Dependency Inversion Principle: Depend on abstractions, not implementations.

### DRY (Don't Repeat Yourself):

   Avoid code duplication. Use reusable functions, classes or modules.

### KISS (Keep It Simple, Stupid):

   Keep your code simple and easy to understand.

### YAGNI (You Aren't Gonna Need It):

   Don't add features until you need them.

### Automated Testing:

   Use unit, integration, and end-to-end tests to ensure code quality.

### Testing Frameworks:

- **Python: pytest, unittest**.

- **Java: JUnit, Mockito**.

- **JavaScript/TypeScript: Jest, Mocha**.

- **Kotlin: KotlinTest, Spek**.

- **Go: testing package**.

- **Rust: cargo test**.

- **PHP: PHPUnit**.

- **C#: xUnit, NUnit**.

- **Scala: ScalaTest**.

- **Haskell: HUnit**.

## 🔥 Features
- **User management** (Create, Read, Update, Delete users)
- **Task management** (CRUD tasks for users)
- **Database integration** (PostgreSQL, SQLite, or similar depending on the stack)
- **REST API endpoints** with documentation (Swagger/OpenAPI)

## 🚀 How to Use
1. **Clone the repository**
   ```bash
   git clone https://github.com/0xrubusdata/TaskManagerCobaye
   cd TaskManagerCobaye
   ```
2. **Checkout a specific implementation**
   ```bash
   git checkout <branch_name>
   ```
   Example:
   ```bash
   git checkout springboot
   ```
3. **Run the application** using Docker Compose
   ```bash
   docker-compose up --build
   ```

## 🛠️ Repository Structure
Each branch contains:
- **Source code** for the specific implementation.
- **Docker configuration** (`docker-compose.yml` and `Dockerfile`).
- **Instructions for running and testing** the stack.

## 🤝 Contribution
Want to add a new language? Fork the repo, create a branch, and submit a PR!

## 📜 License
This project is open-source and available under the MIT License.

---
💡 **Why this project?**
TaskManagerCobaye allows developers to explore different programming paradigms, frameworks, and best practices in building a simple yet functional **Task Manager API** across various stacks. 🚀

