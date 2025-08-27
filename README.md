# Todo App — Java (Spring Boot)
📝 A Todo app implemented in Java Spring Boot, showcasing REST APIs, JPA for database access, and Spring’s dependency injection. This project is part of a series where the same app is built in multiple frameworks (Laravel, Rails, Scotty, .NET) to explore differences in language, architecture, and developer experience.

This is the **Java + Spring Boot implementation** of the [**Multi-Framework Todo App**](https://github.com/JoaoVLima/MultiFrameworkTodoApp) project.

The goal of the overall project is to implement the same simple **Todo List application** across multiple programming languages and web frameworks, in order to **compare architectures, developer experiences, and trade-offs**.

---

## 🚀 Project Overview

The Todo App is a minimal CRUD application.
Features:

* List all todos
* View a single todo
* Create a new todo
* Update an existing todo
* Delete a todo

---

## ☕ Why Java + Spring Boot?

Spring Boot is a powerful framework widely used in enterprise environments. It provides:

* Strong **type safety**
* **Dependency injection** out of the box
* Easy **REST API development**
* Built-in integration with databases via **Spring Data JPA**
* Production-ready tooling (packaging, monitoring, metrics)

Compared to other frameworks in this series, Spring Boot may require more setup and boilerplate, but it excels in **large-scale, maintainable, and team-oriented projects**.

---

## 📂 Project Structure

```
springboot-todo/
 ├── src/main/java/com/example/todo
 │    ├── model/         # Todo entity
 │    ├── repository/    # Data access (JPA)
 │    ├── controller/    # REST API endpoints
 │    └── TodoApp.java   # Main application
 ├── src/main/resources/
 │    └── application.properties  # Config
 └── README.md
```

---

## ⚡ Getting Started

### Prerequisites

* Java 17+
* Maven 3.8+
* SQLite (or another database configured in `application.properties`)

### Run the app

```bash
# Clone the repo
git clone https://github.com/JoaoVLima/springboot-todo.git
cd springboot-todo

# Run with Maven
./mvnw spring-boot:run
```

The app will be available at:
👉 `http://localhost:8080/todos`

---

## 🛠 API Endpoints

| Method | Endpoint      | Description       |
| ------ | ------------- | ----------------- |
| GET    | `/todos`      | List all todos    |
| GET    | `/todos/{id}` | Get a single todo |
| POST   | `/todos`      | Create a new todo |
| PUT    | `/todos/{id}` | Update a todo     |
| DELETE | `/todos/{id}` | Delete a todo     |

---

## 🔑 Reflection Points (Spring Boot)

* ✅ Strong and scalable enterprise framework
* ✅ Type-safe and well-structured
* ⚠️ More boilerplate compared to other frameworks
* ⚡ Best suited for **large teams & long-term projects**

---
