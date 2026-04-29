# 🏨 Perwira Dorm Storage System

A robust web application built with **Laravel** to manage dormitory storage logistics. This system allows students to apply for storage space and helps administrators manage inventory and records.

---

## 🛠 Prerequisites

Ensure you have the following installed before proceeding:

* **XAMPP** (PHP 8.1+ & MySQL)
* **Composer** (PHP Package Manager)
* **Node.js & NPM** (Frontend Asset Manager)
* **Git**

---

## 🚀 Installation & Setup

Follow these steps carefully to get the project running on your local machine:

### 1. Clone the Project
Open your terminal (PowerShell or Git Bash) and run:
```bash
git clone [https://github.com/Yogenn14/dbproject-perwira-dorm-storage-system.git](https://github.com/Yogenn14/dbproject-perwira-dorm-storage-system.git)
cd dbproject-perwira-dorm-storage-system
composer install --ignore-platform-reqs

npm install
cp .env.example .env
php artisan key:generate
```

Start Apache and MySQL in the XAMPP Control Panel.

Go to http://localhost/phpmyadmin and create a new database.

Run the migrations:

```bash

php artisan migrate
```

Terminal,Command,Purpose
Terminal A,
```bash
php artisan serve
```
Starts the PHP Backend (Port 8000)
Terminal B,
```bash
npm run dev
```
Starts the Vite Frontend (Port 5173)
