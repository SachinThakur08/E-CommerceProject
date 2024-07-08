
📚 Product Management System
This project is designed to manage book information, providing functionalities to add, view, edit, and delete book details. The system ensures data integrity by disallowing duplicate ISBN entries. All data is stored in an Oracle database.

🚀 Tech Stack
Spring Boot MVC
Dependencies:
Spring Boot Data JPA
Lombok
JSP
Spring Dev Tools
Spring Web Starter
Oracle Database
Bootstrap for a better UI
🔧 Features
Add Book Information:
Book ISBN
Book Name
Book Author
View Books:
Display the list of added books.
Edit Book:
Modify book details based on ISBN.
Delete Book:
Remove book information based on ISBN.
Validation:
Duplicate ISBN entries are not allowed.
🏗️ Architecture
The project follows a layered architecture, ensuring a clear separation of concerns:

Controller Layer: Handles incoming requests and maps them to the appropriate services.
Service Layer: Contains business logic and manages transactions.
AOP (Aspect-Oriented Programming): Handles cross-cutting concerns such as logging and security.
Exception Layer: Manages and processes exceptions.
Model Layer: Represents the data structure.
Repository Layer: Manages data persistence and retrieval.
📖 Project Explanation
Overview
This product management system is a backend application built with Spring Boot MVC, designed to manage book information efficiently. It allows users to perform CRUD (Create, Read, Update, Delete) operations on book records.

Adding Books
Users can add new books by providing the book's ISBN, name, and author. The system ensures that each ISBN is unique to maintain data integrity.

Viewing Books
Users can view a list of all books added to the system. This feature helps in keeping track of the book inventory.

Editing Books
If there is a need to update the details of a book, users can do so by editing the book information based on the ISBN. This ensures that updates are accurately applied to the correct book.

Deleting Books
Users can remove a book from the system by deleting the book information based on the ISBN. This feature helps in maintaining an up-to-date record of available books.

Validation
The system includes validation mechanisms to prevent duplicate ISBN entries, ensuring that each book in the database has a unique identifier.

Architecture Details
Controller Layer: This layer is responsible for handling HTTP requests and responses. It routes the requests to the appropriate service methods.
Service Layer: This layer contains the core business logic. It processes the data received from the controller and interacts with the repository layer to perform database operations.
AOP (Aspect-Oriented Programming): This aspect-oriented approach handles cross-cutting concerns such as logging and security without cluttering the core business logic.
Exception Layer: This layer deals with exception handling, ensuring that the system can gracefully handle errors and provide meaningful feedback to the users.
Model Layer: This layer represents the data structure of the application. It includes the entity classes that map to the database tables.
Repository Layer: This layer interacts with the database using Spring Data JPA, managing data persistence and retrieval.
