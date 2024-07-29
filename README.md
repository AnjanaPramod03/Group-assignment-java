# Employee Management System CRUD Application

This is a group project developed for [Enterprises Architecture]. The project aims to develop a simple CRUD (Create, Read, Update, Delete) application for managing employee records. It is developed using Java with NetBeans as the IDE, Java Swing for the user interface, and MySQL for the database.

## Group Members

- `KEG/IT/2021/F/0041` - Sandun LB
- `KEG/IT/2021/F/0043` - Anjana
- `KEG/IT/2021/F/0090` - Maduranga
- `KEG/IT/2021/F/0120` - Sahan

## Features

- **Create**: Ability to add new employee records to the database.
- **Read**: View existing employee records.
- **Update**: Modify information of existing employee records.
- **Delete**: Remove employee records from the database.
- **GUI**: User-friendly graphical user interface built using Java Swing.
- **Database**: MySQL database backend for storing employee data.

## Tools Used

- **Java**: Programming language used for the application logic.
- **NetBeans**: Integrated Development Environment (IDE) for Java development.
- **Java Swing**: Toolkit for building graphical user interfaces in Java.
- **MySQL**: Relational database management system for storing employee data.

## Setup Instructions

1. **Clone the repository**
    ```sh
    git clone https://github.com/yourusername/employee-management-system.git
    cd employee-management-system
    ```

2. **Set up the MySQL Database**
    - Create a database named `employee_db`.
    - Use the provided SQL script to create the necessary tables.

    ```sql
    CREATE DATABASE employee_db;
    USE employee_db;

    CREATE TABLE employees (
        id INT AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR(100) NOT NULL,
        position VARCHAR(50),
        salary DECIMAL(10, 2)
    );
    ```

3. **Open the project in NetBeans**
    - Open NetBeans IDE.
    - Click on `File > Open Project` and select the cloned repository.

4. **Configure the database connection**
    - In the project, navigate to `src/com/yourpackage/DatabaseConnection.java`.
    - Update the connection details:
    
    ```java
    String url = "jdbc:mysql://localhost:3306/employee_db";
    String user = "your_mysql_username";
    String password = "your_mysql_password";
    ```

5. **Run the Application**
    - Right-click on the project in NetBeans.
    - Select `Run`.

## Usage

- **Add Employee**: Fill in the employee details in the form and click `Add`.
- **View Employees**: Click on `View All` to see the list of all employees.
- **Update Employee**: Select an employee from the list, modify the details, and click `Update`.
- **Delete Employee**: Select an employee from the list and click `Delete`.
