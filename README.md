
# E-Commerce Employee Database

This repository contains a comprehensive SQL database for an e-commerce company's employee management system. The database includes tables for departments, employees, salaries, titles, and department assignments.

## 📌 Table of Contents
- [Database Schema](#-database-schema)
- [Features](#-features)
- [Installation](#-installation)
- [Usage Examples](#-usage-examples)
- [Data Overview](#-data-overview)
- [Contributing](#-contributing)
- [License](#-license)

## 🗄️ Database Schema

### Tables Structure

1. **`departments`**
   - `dept_no` (CHAR(4), Primary Key)
   - `dept_name` (VARCHAR(40), Unique)

2. **`employees`**
   - `emp_no` (INT, Primary Key)
   - `birth_date` (DATE)
   - `first_name` (VARCHAR(14))
   - `last_name` (VARCHAR(16))
   - `gender` (ENUM('M','F'))
   - `hire_date` (DATE)

3. **`dept_emp`**
   - `emp_no` (INT, Foreign Key to employees)
   - `dept_no` (CHAR(4), Foreign Key to departments)
   - `from_date` (DATE)
   - `to_date` (DATE)

4. **`salaries`**
   - `emp_no` (INT, Foreign Key to employees)
   - `salary` (INT)
   - `from_date` (DATE)
   - `to_date` (DATE)

5. **`titles`**
   - `emp_no` (INT, Foreign Key to employees)
   - `title` (VARCHAR(50))
   - `from_date` (DATE)
   - `to_date` (DATE)

### Views

- **`department_summary`**: Shows total employees per department

## ✨ Features

- Complete employee records with personal and professional details
- Department management system
- Salary history tracking
- Employee title/position tracking
- Department assignment history
- Optimized with indexes for better performance
- Foreign key constraints for data integrity

## 🛠️ Installation

1. Clone this repository:
   ```bash
   [git clone https://github.com/yourusername/ecommerce-employee-db.git
   cd ecommerce-employee-db](https://github.com/Ajal02/new_sql_qry)
