# Sales-Database-Management
in this i am using a database in which have total desciption about sales and how to manage and filter all data .

# 📊 Sales Database Management System (SQL)

A complete SQL-based project for managing and analyzing sales data.  
This project includes database schema creation, sample data insertion, and multiple analytical SQL queries.

---

## 🚀 Features

- Customer Management  
- Product Management  
- Sales Transaction Management  
- Daily / Monthly / Total Sales Reports  
- Top Selling Product Analysis  
- Customer Purchase Summary  
- Automatic Sales Ranking  
- Clean and scalable database schema  

---

## 🗂 Database Schema

The database contains the following tables:

### 1. `customers`
| Column        | Type         | Description           |
|---------------|--------------|-----------------------|
| customer_id   | INT (PK)     | Unique ID             |
| customer_name | VARCHAR      | Customer Full Name    |
| phone         | VARCHAR      | Mobile Number         |
| city          | VARCHAR      | Customer City         |

### 2. `products`
| Column        | Type         | Description           |
|---------------|--------------|-----------------------|
| product_id    | INT (PK)     | Unique Product ID     |
| product_name  | VARCHAR      | Name of Product       |
| price         | DECIMAL      | Product Price         |

### 3. `sales`
| Column        | Type         | Description           |
|---------------|--------------|-----------------------|
| sales_id      | INT (PK)     | Sales transaction ID  |
| customer_id   | INT (FK)     | Customer reference    |
| product_id    | INT (FK)     | Product reference     |
| quantity      | INT          | Units sold            |
| total_amount  | DECIMAL      | Calculated Amount     |
| sale_date     | DATE         | Date of Sale          |

---

## 📁 SQL Files Included

### ✔ `sales_schema.sql`
Contains complete table creation script  
(including PK, FK, Indexes)

### ✔ `sample_data.sql`
Contains sample dummy records for testing the database

### ✔ `queries.sql`
Includes 20+ commonly used analytical SQL queries:
- Daily sales  
- Monthly sales  
- Customer-wise total purchase  
- Top 5 selling products  
- Product-wise revenue  
- Highest purchase customer  
- Sale ranking  
- Duplicate-safe ranking  
- Date-range sales  

---

## 🔧 How to Use

### **1️⃣ Import the Schema**
```sql
SOURCE database/sales_schema.sql;

