# CRAFTPANEL – Minecraft Server Management System

LINK to the gdrive: https://drive.google.com/drive/folders/1Wsu0xy10DfJJZjHTW923iQzGh48lTmr8?usp=sharing


CRAFTPANEL is a full-stack Laravel + Vue 3 web app that simulates a Minecraft-inspired server management system.  
It includes role-based dashboards for Players, World Owners, and Admins.

---

## 📦 Tech Stack

- **Laravel 10** (PHP backend)
- **Vue 3** with Inertia.js (SPA frontend)
- **Vite** (asset bundler)
- **Tailwind CSS** (styling)
- **MySQL** (database)

---

## 🚀 Features

- Authentication (Login, Registration, Logout)
- Player Dashboard with:
  - Profile + Edit Profile
  - World joining, quest tracking, leaderboards
- World Owner Dashboard with:
  - World creation, editing, viewing players
- Admin Dashboard (WIP)
- Friend system (WIP)
- Responsive UI with Minecraft-themed styling

---

## 🛠 Installation & Setup

### 1. Download the project

check the gdrive and download the zip file and extract it into a working folder: e.g., C:\xampp\htdocs\
Open XAMPP and start Apache and MySQL.
go to http://localhost/phpmyadmin in a browser.
Create a new database named mcserverdb.
Import the provided .sql file (from your Google Drive folder):(in the foler called DATABASE_FILE)
Click the Import tab and upload your .sql file.

2. Install PHP dependencies
Go to the Project Directory (cd path-to-project-folder)
composer install

3. Install Node.js dependencies
npm install
4. Environment setup
cp .env.example .env
-Then open .env and set the database credentials:
DB_DATABASE=mcserverdb
DB_USERNAME=root
DB_PASSWORD=    # leave blank if no MySQL password is set in XAMPP
-Generate app key:
php artisan key:generate
5. Migrate the database
php artisan migrate
6. Run the server
php artisan serve
npm run dev

Now visit http://localhost:8000
