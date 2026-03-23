# 🚀 Dynamic Pricing and Demand Intelligence System

## 👩‍💻 Developed By
- Kashish
- BCA Student

🏫 Meerut Institute of Technology  
👨‍🏫 Guide: Rahul Singh  

---

## 📌 Project Description
This project demonstrates a **Dynamic Pricing System** where product prices are automatically adjusted based on customer demand using MySQL.

---

## 🎯 Objective
- Analyze product demand  
- Adjust prices dynamically  
- Simulate real-world pricing strategies  

---

## 🛠️ Technologies Used
- MySQL  
- MySQL Workbench  

---

## 🗄️ Database Structure

### 📦 Products Table
- product_id (Primary Key)  
- base_price  
- current_price  

### 🛒 Sales Table
- sale_id (Primary Key)  
- product_id (Foreign Key)  
- quantity  
- sale_date  

---

## 🔗 Relationship
- One product can have multiple sales  
- Connected using **product_id**

---

## ⚙️ Working Process
1. Calculate demand using:
   - `SUM()`  
   - `GROUP BY`  

2. Apply pricing logic using:
   - `CASE` statement  

---

## 💡 Pricing Logic
- Demand > 10 → 🔼 Increase price by 10%  
- Demand < 5 → 🔽 Decrease price by 10%  
- Else → ➖ No change  

---

## 📊 Sample Output
| Product     | Demand |
|------------|--------|
| Headphones | 20     |
| Laptop     | 15     |
| Mobile     | 2      |

---

## ✨ Features
- Dynamic pricing system  
- Demand analysis  
- Real-time price updates  
- SQL-based logic  

---

## ⚠️ Challenges Faced
- Error Code 1175 (Safe Update Mode)  
✔️ Resolved using:
```sql
SET SQL_SAFE_UPDATES = 0;
