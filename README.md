

# Airline Reservation System Project in Java

## Introduction
In this article, we will build an **Airline Reservation System Project** using Java and MySQL with source code. This project is perfect for those at an intermediate level in Java who wish to enhance their coding skills. The users can perform various functionalities such as accessing the Home Page, Registration, Viewing Flight Details, and Booking Tickets. Let’s get started!

## Setting Up the Development Environment

### Prerequisites
- **Java JDK**: Ensure Java JDK is installed on your system.
- **IDE**: We recommend using **Eclipse IDE** for this project, though **NetBeans** can also be used.
- **MySQL**: Install MySQL on your system.
- **MySQL Connector**: Download the MySQL connector.

### Steps to Setup
1. **Create a New Project**: Start by creating a new project in your IDE and name it as desired.
2. **Package Creation**: In the `src` folder, create a package named `airline`. This package will contain different files for various modules.
3. **Database Connection**:
    - Download the MySQL connector.
    - In Eclipse, under your project, expand **External Libraries**.
    - Right-click, select **Open Library Settings**, then select the **Libraries** tab.
    - Click the **+** button, browse to the downloaded jar file, and add it as a dependency to your project.
    - Steps may differ if using a different IDE.

## MySQL Setup for Airline Reservation System Project in Java

### Database Creation
1. **Create a Database**:
    ```sql
    CREATE DATABASE airline;
    ```

2. **Select the Database**:
    ```sql
    USE airline;
    ```

3. **Create Flights Table**:
    ```sql
    CREATE TABLE flights (
        flight_id INT PRIMARY KEY,
        flight_name VARCHAR(25),
        fdate DATE,
        time VARCHAR(10),
        class VARCHAR(10)
    );
    ```

4. **Create Register Table**:
    ```sql
    CREATE TABLE register (
        passenger_id INT PRIMARY KEY,
        first_name VARCHAR(25),
        last_name VARCHAR(25),
        contact_no VARCHAR(10),
        address VARCHAR(250),
        email VARCHAR(25)
    );
    ```

## Project Modules

### 1. Home Page Module
- **Description**: After entering the correct username and password on the login page, the user is directed to the home page of the airline reservation system.
- **File Name**: `main.java`

### 2. Registration Module
- **Description**: This module allows the addition of new passenger details. It also provides functionalities to edit or delete existing passenger records.
- **File Name**: `Registration.java`

### 3. Flights Module
- **Description**: This module displays flight details.
- **File Name**: `Flights.java`

### 4. Booking Module
- **Description**: This module helps in booking tickets.
- **File Name**: `Booking.java`

## Conclusion
In this project, we developed a GUI-based **Airline Reservation System** using Java and MySQL. The application allows users to perform essential operations such as accessing the Home Page, Registration, Viewing Flight Details, and Booking Tickets. We recommend adding more modules and functionalities to make this airline reservation system more comprehensive and applicable to real-world scenarios.

---

