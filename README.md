# dbproject-perwira-dorm-storage-system

Perwira Dorm Storage System
This is a web-based storage management application built with the Laravel framework. This system allows students to manage their belongings and dormitory staff to oversee storage logistics.

🛠 Prerequisites
Before starting, ensure you have the following software installed:

XAMPP (PHP 8.1 or higher & MySQL)

Composer (PHP Package Manager)

Node.js & NPM (Frontend Asset Manager)

Git

🚀 Installation & Setup
1. Clone the Project
Open your terminal and run:

Bash
git clone https://github.com/Yogenn14/dbproject-perwira-dorm-storage-system.git
cd dbproject-perwira-dorm-storage-system
2. Install PHP Dependencies
If you have a newer version of PHP (like 8.2 or 8.3), use the ignore flag:

Bash
composer install --ignore-platform-reqs
3. Install Frontend Dependencies
Bash
npm install
4. Configure Environment
Create your local .env file from the template:

Bash
cp .env.example .env
php artisan key:generate
Note: Open the .env file in VS Code and ensure DB_DATABASE matches the name of the database you create in XAMPP (e.g., perwira_dorm).

5. Database Setup
Start Apache and MySQL in your XAMPP Control Panel.

Go to http://localhost/phpmyadmin and create a new database.

Run the migrations to create the tables:

Bash
php artisan migrate
⚠️ Troubleshooting (Common Fixes)
Missing Extensions (fileinfo, gd, zip)
If Composer gives an error about missing extensions, you must enable them in XAMPP:

Open C:\xampp\php\php.ini.

Remove the semicolon (;) from the start of these lines:

extension=fileinfo

extension=gd

extension=zip

Restart your terminal and XAMPP.

"mysqli.so" Warning on Windows
If you see a warning about a .so library:

Open php.ini.

Delete any line that contains /path/to/extension/mysqli.so.

Ensure extension_dir = "C:\xampp\php\ext" is correctly set.

🏃 How to Run the App
You must run two terminals at the same time:

Terminal 1 (Backend Server):

Bash
php artisan serve
Terminal 2 (Frontend Assets):

Bash
npm run dev
Access the site at: http://127.0.0.1:8000

📄 License
Developed for the Database Course Project at UTHM.
