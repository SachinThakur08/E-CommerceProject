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
  - **Flash Message:** "New book added successfully"
- **View Books:**
  - Display the list of added books.
- **Edit Book:**
  - Modify book details based on ISBN.
  - **Flash Message:** "Book updated successfully"
- **Delete Book:**
  - Remove book information based on ISBN.
  - **Flash Message:** "Book deleted successfully"
- **Validation:**
  - Duplicate ISBN entries are not allowed.
  - **Flash Message:** "Duplicate ISBN not allowed"

## 🏗️ Architecture

The project follows a layered architecture, ensuring a clear separation of concerns:

- **Controller Layer:** Handles incoming requests and maps them to the appropriate services.
- **Service Layer:** Contains business logic and manages transactions.
- **AOP (Aspect-Oriented Programming):** Handles cross-cutting concerns such as logging and security.
- **Exception Layer:** Manages and processes exceptions.
- **Model Layer:** Represents the data structure.
- **Repository Layer:** Manages data persistence and retrieval.

## Project Explanation

### Overview
This product management system is a backend application built with Spring Boot MVC, designed to manage book information efficiently. It allows users to perform CRUD (Create, Read, Update, Delete) operations on book records.

### Adding Books
Users can add new books by providing the book's ISBN, name, and author. The system ensures that each ISBN is unique to maintain data integrity. A flash message "New book added successfully" confirms the action.

### Viewing Books
Users can view a list of all books added to the system. This feature helps in keeping track of the book inventory.

### Editing Books
If there is a need to update the details of a book, users can do so by editing the book information based on the ISBN. This ensures that updates are accurately applied to the correct book. A flash message "Book updated successfully" confirms the action.

### Deleting Books
Users can remove a book from the system by deleting the book information based on the ISBN. This feature helps in maintaining an up-to-date record of available books. A flash message "Book deleted successfully" confirms the action.

### Validation
The system includes validation mechanisms to prevent duplicate ISBN entries, ensuring that each book in the database has a unique identifier. A flash message "Duplicate ISBN not allowed" indicates when a duplicate ISBN entry is attempted.



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


```
![Presentation1](https://github.com/rohithsomella/product-management/assets/141708838/c19db542-d87b-436e-995a-b83769aaf55e)
