# ✈️ Airline Reservation System Project in Java

> A GUI-based desktop application for booking airline tickets, managing flight details, and handling passenger registrations — built using **Java** and **MySQL**.

---

## 📌 Introduction

This **Airline Reservation System** is a simple yet functional project aimed at intermediate Java learners. It provides a user-friendly interface for flight management, passenger registration, and ticket booking using **Java Swing** and **MySQL** for backend data storage.

---

## 🧰 Technologies Used

| Category       | Technology           |
|----------------|----------------------|
| Programming    | Java (Swing, AWT)    |
| Database       | MySQL                |
| Connectivity   | MySQL Connector/J    |
| IDE Suggested  | Eclipse / NetBeans   |

---

## 🛠️ Setting Up the Development Environment

### ✅ Prerequisites

- 🔹 Java JDK (8 or above)
- 🔹 Eclipse or NetBeans IDE
- 🔹 MySQL Server
- 🔹 MySQL Connector/J (JDBC driver)

---

### 🚀 Setup Instructions

1. **Create a New Project**  
   Open Eclipse and create a new Java project named `AirlineReservationSystem`.

2. **Add Package**  
   Create a package named `airline` under `src`.

3. **Add MySQL Connector**  
   - Download MySQL Connector from [MySQL Official Site](https://dev.mysql.com/downloads/connector/j/).
   - In Eclipse:  
     `Project → Properties → Java Build Path → Libraries → Add External JARs → Select mysql-connector.jar`

4. **Start Coding!**  
   Begin by creating the required Java files inside the `airline` package.

---

## 🗄️ MySQL Database Setup

### 🔧 Step-by-Step SQL Setup

```sql
-- Create the database
CREATE DATABASE airline;

-- Use the created database
USE airline;

-- Create flights table
CREATE TABLE flights (
    flight_id INT PRIMARY KEY,
    flight_name VARCHAR(25),
    fdate DATE,
    time VARCHAR(10),
    class VARCHAR(10)
);

-- Create register table
CREATE TABLE register (
    passenger_id INT PRIMARY KEY,
    first_name VARCHAR(25),
    last_name VARCHAR(25),
    contact_no VARCHAR(10),
    address VARCHAR(250),
    email VARCHAR(25)
);
```

---

## 📦 Project Modules Overview

### 1. 🏠 Home Page Module
- **Description**: Authenticated users are redirected here after login. This is the dashboard of the system.
- **File**: `Main.java`

---

### 2. 📝 Registration Module
- **Description**: Handles new passenger registrations. Includes CRUD functionality for managing passenger records.
- **File**: `Registration.java`

---

### 3. ✈️ Flights Module
- **Description**: Displays all available flight details pulled from the database.
- **File**: `Flights.java`

---

### 4. 🎫 Booking Module
- **Description**: Enables users to book flight tickets with available flight data.
- **File**: `Booking.java`

---

## 📸 Sample GUI Screens (Optional)

> _Add screenshots or GIFs of your application UI to showcase the user interface._

---

## 🧠 Future Enhancements

- ✅ Add login authentication with roles (Admin/Passenger)  
- ✅ Include booking history and cancellation features  
- ✅ Integrate email confirmations  
- ✅ Payment gateway simulation  

---

## ✅ Conclusion

This project offers a hands-on approach to learning **Java GUI development** and **MySQL database integration**. The **Airline Reservation System** is a great starting point for building scalable, modular applications in Java. You can enhance this system further by adding authentication, real-time seat availability, and ticketing options.

---

