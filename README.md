# Todo List API

## Overview
This project is a simple Todo List Web API implemented using .NET Core, designed to demonstrate best practices in API development while adhering to the Clean Architecture principles. The API supports creating, updating, and retrieving Todo items and is implemented with modern tools and patterns for maintainability and scalability.

---

## Features
1. **Core Features:**
    - Create a new Todo item.
    - Mark a Todo item as completed.
    - Retrieve all Todo items.
    - Retrieve completed Todo items.
    - Retrieve pending (not completed) Todo items.
2. **Additional Features:**
    - **CQRS Pattern:** Clear separation of command and query responsibilities.
    - **FluentValidation:** Used for request validation.
    - **Serilog:** Integrated for structured logging.
    - **EF Core 8:** Utilized with an in-memory database for simplicity.
    - **In-Memory Caching:** Caching for improved performance.
    - **API Versioning:** To support future iterations and backward compatibility.
    - **Scrutor:** For streamlined dependency injection.
    - **Unit Tests:** Comprehensive tests using Moq.
    - **Clean Architecture:** Organized into Domain, Application, Infrastructure, and Presentation layers.
    - **Vertical Slicing:** Features grouped for easy maintainability.
    - **Domain-Driven Design (DDD):** Emphasis on domain entities and rich domain modeling.
    - **Auditable and Soft Deletable Entities:** Tracks creation, modification, and deletion metadata.
    - **Generic Repository and Unit of Work Patterns:** Simplifies data access.
    - **Specification Pattern:** For flexible and reusable query filters.
    - **Result Pattern:** Unified approach to handling results and errors.
    - **Localization:** Error messages support multiple languages.
    - Swagger: API documentation for easier interaction and testing.

---

## API Endpoints

### Version: v1.0

| Endpoint                  | HTTP Method | Description                             |
|---------------------------|-------------|-----------------------------------------|
| `/api/v1/todo/add-item`            | POST        | Create a new Todo item.                |
| `/api/v1/todo/get-all-items`            | GET         | Retrieve all Todo items.               |
| `/api/v1/todo/get-completed-items`            | GET         | Retrieve all completed Todo items.               |
| `/api/v1/todo/get-pending-items`    | GET         | Retrieve all pending Todo items.       |
| `/api/v1/todo/complete-item/{id}` | PUT      | Mark a Todo item as completed.         |

---

## Tech Stack
- **.NET 8**: Latest framework features.
- **Entity Framework Core 8**: Simplified data access.
- **FluentValidation**: Validation for request models.
- **Serilog**: Enhanced logging.
- **Swagger**: Auto-generated API documentation.
- **Moq**: Unit testing with mocked dependencies.

---

## Architecture
- **Domain Layer:** entities.
- **Application Layer:** Handles CQRS, validation, and DTO mappings.
- **Infrastructure Layer:** Implements caching, sedder, and external integrations.
- **Persistence Layer:** Implements data persistence, database tables configurations and migrations.
- **Presentation Layer:** API controllers.
---

## Author
Mohamed Mohanad

