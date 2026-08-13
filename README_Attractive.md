# 📝 Todo Management System

> A clean and simple task management web application built with **Java + Spring Boot**, with **MySQL** for persistent data storage.

<p align="center">
  <b>Java</b> • <b>Spring Boot</b> • <b>Spring Data JPA</b> • <b>MySQL</b> • <b>Thymeleaf</b> • <b>Lombok</b>
</p>

---

## ✨ Features

- ➕ **Add Tasks** — Create new todo tasks
- 📋 **View Tasks** — Display saved tasks
- ✏️ **Update Tasks** — Modify task details
- ✅ **Complete Tasks** — Mark tasks as completed
- 🗑️ **Delete Tasks** — Remove tasks
- 💾 **Persistent Storage** — Store task data in MySQL

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| ☕ **Java** | Core programming language |
| 🌱 **Spring Boot** | Application framework |
| 🌐 **Spring Web** | Handles web requests and controllers |
| 🗃️ **Spring Data JPA** | Database persistence and CRUD operations |
| 🐬 **MySQL** | Relational database |
| 🎨 **Thymeleaf** | Server-side HTML rendering |
| ♻️ **Lombok** | Reduces Java boilerplate code |
| 📦 **Maven** | Project build and dependency management |

---

## 🏗️ Application Architecture

The project follows a layered architecture to keep request handling, business logic, and database access separated.

```text
                    🌐 Browser
                        │
                        ▼
                ┌───────────────┐
                │   Controller  │
                └───────┬───────┘
                        │
                        ▼
                ┌───────────────┐
                │    Service    │
                └───────┬───────┘
                        │
                        ▼
                ┌───────────────┐
                │   Repository  │
                └───────┬───────┘
                        │
                        ▼
             ┌─────────────────────┐
             │ Spring Data JPA /   │
             │ Hibernate           │
             └──────────┬──────────┘
                        │
                        ▼
                  🐬 MySQL
```

### 📌 Layer Responsibilities

**Controller**
- Receives HTTP requests
- Maps requests to application actions
- Returns the appropriate response/view

**Service**
- Contains application/business logic
- Acts as the bridge between Controller and Repository

**Repository**
- Handles database interaction
- Uses Spring Data JPA for CRUD operations

**Entity / Model**
- Represents task data
- Maps Java objects to database records

**Thymeleaf**
- Renders dynamic HTML pages on the server side

---

## 🔄 CRUD Operations

| Operation | Function |
|---|---|
| 🟢 **Create** | Add a new task |
| 🔵 **Read** | Fetch and display tasks |
| 🟡 **Update** | Modify task information |
| 🔴 **Delete** | Remove a task |

---

## 🗄️ Database

The application uses **MySQL** to persist task data.

Spring Data JPA is used to interact with the database without writing every SQL query manually.

Example configuration:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/your_database
spring.datasource.username=your_username
spring.datasource.password=your_password
```

> ⚠️ **Security:** Never push your actual database password or other secrets to GitHub. Use environment variables or a local configuration file for sensitive values.

---

## 🚀 Getting Started

### Prerequisites

Make sure the following are installed:

- ☕ Java JDK
- 📦 Maven
- 🐬 MySQL
- 🔧 Git

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd <project-folder>
```

### 2. Create the database

Create a MySQL database and configure the application's database properties.

### 3. Configure MySQL

Update your local database credentials:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/your_database
spring.datasource.username=your_username
spring.datasource.password=your_password
```

### 4. Run the application

Using Maven:

```bash
mvn spring-boot:run
```

Or run the main Spring Boot application class from your IDE.

### 5. Open the application

Open the local application URL shown by Spring Boot in your browser.

---

## 📚 What I Learned

Building this project helped me practice:

- Java and object-oriented programming
- Spring Boot application development
- MVC-style web application structure
- Controller → Service → Repository architecture
- CRUD operations
- Spring Data JPA
- MySQL database integration
- Entity and primary-key mapping
- Thymeleaf server-side rendering
- Lombok
- Maven project management

---

## 🔮 Future Improvements

Some features that can be added in future versions:

- 👤 User authentication and authorization
- 🏷️ Task categories and priorities
- 📅 Due dates and reminders
- 🔎 Search and filtering
- 🔌 REST API endpoints
- 📱 Responsive UI improvements

---

## 👨‍💻 Author

### Rohit Kumar

**B.Tech — Computer Science Engineering**

🔗 **GitHub:** [rohitkumar2702](https://github.com/rohitkumar2702)

🔗 **LinkedIn:** [Rohit Kumar](https://www.linkedin.com/in/rohit-kumar-611456306)

---

⭐ **If you found this project useful, consider giving the repository a star!**
