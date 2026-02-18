
# 📚 Library Management System (SQL Project)

## 📌 Project Overview

**Project Name:** Library Management System  
**Level:** Intermediate  
**Database:** `library_db`  

This project demonstrates the design and implementation of a **Library Management System using SQL**. It covers database creation, relational modeling, CRUD operations, stored procedures, reporting, and advanced SQL queries.

The goal of this project is to showcase practical SQL skills used in real-world database systems.

---

## 🎯 Objectives

- Design a relational database for a library system
- Implement proper table relationships and constraints
- Perform CRUD operations
- Use CTAS (Create Table As Select)
- Write advanced SQL queries for reporting and analysis
- Create stored procedures to automate business logic

---

## 🏗️ Database Schema

The system consists of the following tables:

- `branch`
- `employees`
- `members`
- `books`
- `issued_status`
- `return_status`

### Entity Relationship Overview

- Each **branch** has multiple employees  
- Each **member** can issue multiple books  
- Each **book** can be issued and returned  
- Each issue record connects:
  - Member
  - Employee
  - Book
- Return records track completed transactions  

---

## 🗄️ Database Setup

```sql
CREATE DATABASE library_db;
```

The project includes:

- Table creation with primary and foreign keys
- Proper relational mapping
- Data integrity constraints

---

# 🔄 CRUD Operations

### ✅ Create
Insert new book records into the `books` table.

### 📖 Read
Retrieve records using SELECT queries.

### ✏️ Update
Modify existing records (e.g., update member address).

### ❌ Delete
Remove records such as issued book entries.

---

# 🧠 Core SQL Features Implemented

## 1️⃣ Issue & Return Tracking
- Track issued books  
- Identify returned books  
- Identify unreturned books  

## 2️⃣ Overdue Book Detection
- Identify books issued for more than 30 days  
- Calculate overdue days dynamically  

## 3️⃣ Revenue Analysis
- Calculate rental revenue by category  
- Generate branch-level performance reports  

## 4️⃣ Member Insights
- Members who issued multiple books  
- Recently registered members  
- Active members (last 2 months)  

## 5️⃣ Employee Performance
- Top employees by books processed  
- Employee-branch-manager reporting  

---

# 🏗️ Stored Procedures

## 📘 Issue Book Procedure

- Checks book availability  
- Inserts issue record  
- Updates book status  
- Prevents issuing unavailable books  

## 📕 Return Book Procedure

- Inserts return record  
- Updates book availability  
- Displays confirmation message  

---

# 📊 Reporting Features

## 📌 Branch Performance Report
- Total books issued  
- Total books returned  
- Total revenue generated  

## 📌 Active Members Table (CTAS)
Creates a table of members who issued books within the last 2 months.

## 📌 Overdue & Fine Calculation (CTAS)
- Counts overdue books per member  
- Calculates fine at **$0.50 per day**  
- Generates summarized overdue report  

---

# 🛠️ Advanced SQL Concepts Used

- JOIN (INNER, LEFT)
- GROUP BY & HAVING
- Aggregate Functions (SUM, COUNT)
- Subqueries
- CTAS (CREATE TABLE AS SELECT)
- Stored Procedures (PL/pgSQL)
- Conditional Logic (IF statements)
- Date Arithmetic
- Foreign Key Constraints

---

# 📈 Key Learning Outcomes

✔ Database design & normalization  
✔ Real-world relational modeling  
✔ Writing analytical SQL queries  
✔ Business logic implementation in SQL  
✔ Building summary & reporting tables  
✔ Automating workflows with stored procedures  

---

# 🚀 How to Use

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/najirh/Library-System-Management---P2.git
```

### 2️⃣ Set Up the Database

Run the SQL scripts inside:

- `database_setup.sql`
- `analysis_queries.sql`

### 3️⃣ Explore the System

- Insert sample data  
- Execute analytical queries  
- Modify logic  
- Extend reporting features  

---

# 📌 Possible Enhancements

- Add triggers for automatic fine updates  
- Implement role-based access control  
- Add book inventory quantity tracking  
- Convert to full-stack web application  
- Integrate dashboard (Power BI / Tableau)  

---

# 👨‍💻 Author

**Kishore E**

If you found this project helpful, feel free to connect:
  
- 💼 LinkedIn: (https://www.linkedin.com/in/kishoree23/)   

---

# ⭐ Support

If you like this project:

- ⭐ Star the repository  
- 🍴 Fork it  
- 📢 Share it  

---

## 📚 Conclusion

This project demonstrates intermediate-level SQL skills by building a complete relational database system from scratch. It simulates real-world business logic found in library systems and provides a strong foundation for database development and data analysis roles.
