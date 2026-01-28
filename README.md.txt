# 🎓 Student Management System (Java + JDBC + PostgreSQL)

A **console-based Student Management System** developed using **Core Java and JDBC**, designed to manage student records efficiently with PostgreSQL database integration.

This project demonstrates backend fundamentals including database connectivity, CRUD operations, and clean Java code structure.

---

## 🚀 Features

- ➕ Add new student
- 📋 View all students
- 🔍 Search student by ID
- ✏️ Update student details
- ❌ Delete student record
- 🚪 Exit application safely

---

## 🛠️ Technologies Used

- Java (Core Java)
- JDBC
- PostgreSQL
- SQL
- Eclipse / IntelliJ IDEA
- Git & GitHub

---

## 📂 Project Structure

Student-Management-System/
│
├── src/
│ └── com/
│ └── sms/
│ ├── Dbconnection.java
│ ├── Student.java
│ ├── StudentDao.java
│ └── Main.java
│
├── screenshots/
│ ├── start_output.png
│ ├── add_student.png
│ ├── view_student.png
│ ├── search_student.png
│ ├── update_student.png
│ ├── delete_student.png
│ └── exit.png
│
├── README.md
├── .gitignore


---

## 🖼️ Application Screenshots

### ▶️ Application Start
![Start Output](screenshots/start_output.png)

### ➕ Add Student
![Add Student](screenshots/add_student.png)

### 📋 View Students
![View Student](screenshots/view_student.png)

### 🔍 Search Student
![Search Student](screenshots/search_student.png)

### ✏️ Update Student
![Update Student](screenshots/update_student.png)

### ❌ Delete Student
![Delete Student](screenshots/delete_student.png)

### 🚪 Exit Application
![Exit](screenshots/exit.png)

---

## 🗄️ Database Setup

Create PostgreSQL database:

```sql
CREATE DATABASE smsdb;
Create table:

CREATE TABLE student (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100),
    course VARCHAR(50)
);
🔐 Database Configuration
Update database credentials in Dbconnection.java:

private static final String URL = "jdbc:postgresql://localhost:5432/smsdb";
private static final String USER = "postgres";
private static final String PASSWORD = System.getenv("DB_PASSWORD");
⚠️ Database password is managed using environment variables for security.

▶️ How to Run the Project
Clone the repository

git clone https://github.com/your-username/student-management-system.git
Open project in Eclipse / IntelliJ

Add PostgreSQL JDBC Driver to classpath

Set environment variable:

setx DB_PASSWORD your_password
Run Main.java


⭐ If you like this project, please give it a star!