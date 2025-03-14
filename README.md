#THIS IS AI GENNED. I WAS SEEING WHAT IT COULD DO

# Java JDBC Application with Maven

## Overview
Welcome, students! This repository provides an example Java application designed to help you understand key concepts required for your final sprint project. This program demonstrates how to use JDBC to interact with a PostgreSQL (PG) database using Java through the Command Line Interface (CLI). Please use this example to learn about Maven for dependency management, structuring a Java project using a three-tiered approach, handling user inputs with Scanner, implementing password hashing and user authentication, and storing data in a PostgreSQL database.

## Learning Objectives
- **Dependency Management**: Understand how to use Maven to manage project dependencies.
- **Project Structure**: Learn how to organize your code using a three-tier architecture (Presentation, Business Logic, Data Access).
- **User Input Handling**: Discover how to use Scanner for handling user inputs.
- **Authentication**: Learn about password hashing and implementing user authentication.
- **Database Integration**: Explore how to use JDBC to interact with a PostgreSQL database and manage user and car data.

## Key Concepts
### Dependency Management with Maven
Maven is a powerful tool for managing your project's dependencies. It simplifies the process of including external libraries and ensures that your project uses the correct versions.

### Three-Tier Project Structure
The three-tier architecture separates the application into distinct layers:
- **Presentation Layer**: Manages user interactions and inputs.
    - Example Files: `Main.java`, `Menu.java`
- **Business Logic Layer**: Contains the core application logic.
    - Example Files: `UserService.java`, `CarService.java`
- **Data Access Layer**: Handles interactions with the database.
    - Example Files: `UserDao.java`, `CarDao.java`, `DBConnection.java`

### Handling User Inputs with Scanner
The `Scanner` class is used to handle user inputs efficiently. For instance:
```java
Scanner scanner = new Scanner(System.in);
System.out.print("Enter username: ");
String username = scanner.nextLine();
System.out.print("Enter password: ");
String password = scanner.nextLine();
