# 🧼 Cleaning Tools Shop Web System  
A web-based management system for a cleaning tools shop. The system comes with **two user roles** — **Admin** and **Staff** — each with different permissions to manage products, customers, orders, and staff details.  
Built using **PHP**, **MySQL (phpMyAdmin)**, **HTML/CSS/JS**, and simple CRUD operations.

---

## 🚀 Features

### 🔐 Authentication & Roles
- **Admin**
  - Full CRUD on Products, Customers, Staff, Orders
  - View and update product images
  - Manage all system data  
- **Normal Staff**
  - View-only or limited CRUD (depending on page)
  - Cannot access restricted admin-only pages

---

## 🛒 Modules Overview

### 🧴 Products
- View products list  
- Detailed product page  
- Add, edit, delete product info  
- Product images stored in `/uploads`  
- Display images stored in `/images`

### 👥 Customers
- Customer list & details  
- CRUD operations for Admin  
- Staff has only limited permissions

### 🧑‍💼 Staffs
- Admin can manage staff records  
- Staff can only view their own info (if implemented)

### 📦 Orders
- View orders  
- Add, edit, delete order details  
- Order details stored in related tables

---

## 📁 Project Directory Structure

```bash
project/
│── public/
│   ├── index.php
│   ├── login.php
│   ├── logout.php
│   ├── customers.php
│   ├── customers_crud.php
│   ├── invoice.php
│   ├── orders.php
│   ├── orders_crud.php
│   ├── orders_details.php
│   ├── orders_details_crud.php
│   ├── products.php
│   ├── products_crud.php
│   ├── products_details.php
│   ├── staffs.php
│   ├── staffs_crud.php
│   ├── login_process.php
│   ├── nav_bar.php
│   └── logo.png
│
│── src/
│   └── database.php
│
│── assets/
│   ├── css/
│   ├── js/
│   ├── images/
│   ├── pictures/
│   └── fonts/
│
│── uploads/
│
│── config/
│   └── path.php
│
│── README.md
└── .gitignore
```


---

## 🗄️ Database

- Database created using **phpMyAdmin**
- Connected through `database.php`
- Includes tables:
  - `products`
  - `customers`
  - `staffs`
  - `orders`
  - `order_details`

---

## 📷 Image Management

- New product images are stored in **`/uploads`**
- Existing/initial images are in **`/images`**
- File upload handled inside product CRUD pages

---

## ⚙️ How to Run the Project

1. Clone the repository  
   ```bash
   git clone https://github.com/yourusername/your-repo.git
   
2. Move project folder into your local server directory:
XAMPP: htdocs/

3. Import the database:
Go to phpMyAdmin
Create a new database

4. Start Apache & MySQL
Visit in browser:
http://localhost/your-folder/


