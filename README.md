# 📚 Product Management System

This project is designed to manage book information, providing functionalities to add, view, edit, and delete book details. The system ensures data integrity by disallowing duplicate ISBN entries. All data is stored in an Oracle database.

## 🚀 Tech Stack

- **Spring Boot MVC**
  - **Dependencies:**
    - Spring Boot Data JPA
    - Lombok
    - JSP
    - Spring Dev Tools
    - Spring Web Starter
  - Oracle Database
  - Bootstrap for a better UI

## 🔧 Features

- **Add Book Information:**
  - Book ISBN
  - Book Name
  - Book Author
- **View Books:**
  - Display the list of added books.
- **Edit Book:**
  - Modify book details based on ISBN.
- **Delete Book:**
  - Remove book information based on ISBN.
- **Validation:**
  - Duplicate ISBN entries are not allowed.

## 🏗️ Architecture

The project follows a layered architecture, ensuring a clear separation of concerns:

- **Controller Layer:** Handles incoming requests and maps them to the appropriate services.
- **Service Layer:** Contains business logic and manages transactions.
- **AOP (Aspect-Oriented Programming):** Handles cross-cutting concerns such as logging and security.
- **Exception Layer:** Manages and processes exceptions.
- **Model Layer:** Represents the data structure.
- **Repository Layer:** Manages data persistence and retrieval.

## 📂 Project Structure

```plaintext
Spring-MVC-Project-OracleDB/
│
├── .classpath
├── .factorypath
├── .gitignore
├── .project
├── HELP.md
├── mvnw
├── mvnw.cmd
├── pom.xml
│
├── .mvn/
│   └── wrapper/
│       ├── maven-wrapper.jar
│       └── maven-wrapper.properties
│
└── src/
    ├── main/
    │   ├── java/
    │   │   └── com/
    │   │       └── boot/
    │   │           └── project/
    │   │               ├── SpringMvcProjectApplication.java
    │   │               ├── aop/
    │   │               │   └── BookControllerAdvice.java
    │   │               ├── controller/
    │   │               │   └── BookController.java
    │   │               ├── exception/
    │   │               │   └── DuplicateBookException.java
    │   │               ├── model/
    │   │               │   └── Book.java
    │   │               ├── repository/
    │   │               │   └── BookRepository.java
    │   │               └── service/
    │   │                   └── BookService.java
    │   ├── resources/
    │   │   ├── application.properties
    │   │   └── static/
    │   │       └── images/
    │   │           ├── bg.jpg
    │   │           ├── bg2.jpg
    │   │           ├── bg3.jpg
    │   │           └── bg4.jpg
    │   └── webapp/
    │       └── WEB-INF/
    │           └── views/
    │               └── book.jsp
    │
    └── test/
        └── java/
            └── com/
                └── boot/
                    └── project/
                        └── SpringMvcProjectApplicationTests.java
