<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7f1d1d,100:ef4444&height=170&section=header&text=Social%20Media%20Platform&fontColor=ffffff&fontSize=44&fontAlignY=38&desc=A%20PHP%20and%20MySQL%20social%20feed%20project&descAlignY=60&descSize=16" alt="Social Media Platform in PHP" />

![PHP](https://img.shields.io/badge/PHP-7-777bb4?style=flat-square&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-database-4479a1?style=flat-square&logo=mysql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-f7df1e?style=flat-square&logo=javascript&logoColor=black)
![AJAX](https://img.shields.io/badge/AJAX-interactions-333333?style=flat-square)

</div>

A server-rendered social platform project built with PHP and MySQL. It includes account flows, user profiles, a post feed, and supporting social interactions implemented across PHP pages and classes.

## ✨ Features

- User signup, login, logout, and profile pages.
- Create posts with text and image uploads; view individual posts and comments.
- Follow-related content, likes, and notifications.
- Profile sections for photos, followers/following, about details, and settings.
- Search pages, pagination helpers, and AJAX endpoints for interactions.
- `mybook_db.sql` provides the MySQL schema and sample rows.

## 🏗️ Architecture

PHP pages handle routing and rendering, reusable classes in `classes/` contain account, post, profile, and notification logic, and `classes/connect.php` connects to MySQL. Browser requests use PHP endpoints (including `ajax/`) for interactive actions. Uploaded images are stored under `uploads/`.

## 🧰 Tech stack

| Area | Technology |
| --- | --- |
| Server | PHP |
| Database | MySQL / MariaDB with `mysqli` |
| Browser | HTML, CSS, JavaScript, AJAX |
| Local web server | Apache or another PHP-capable server |

## 🚀 Getting started

1. Install PHP with the `mysqli` extension, MySQL or MariaDB, and a local PHP web server (for example, XAMPP).
2. Create a database named `mybook_db` and import `mybook_db.sql` using phpMyAdmin or the MySQL client.
3. Review `classes/connect.php` and set the database host, username, password, and database name for your local environment. The committed defaults are local-development credentials.
4. Serve the repository from the web server's document root, then open the project in a browser.
5. Ensure the web server can write to `uploads/` if you use image-upload features.

The SQL dump contains insert statements as well as table definitions, so inspect sample data before importing into a shared or production database.

## 📁 Project structure

```text
├── index.php             # Main feed
├── signup.php / login.php
├── profile.php           # Profile views and sections
├── classes/              # Database and application classes
├── ajax/                 # AJAX interaction handlers
├── uploads/              # User-uploaded media location
└── mybook_db.sql         # Schema and sample data
```

## 🗺️ Roadmap / Notes

- This is a traditional PHP learning project; the database connection is hard-coded for local use and should be configured before running elsewhere.
- No dependency manifest, automated test suite, or production deployment configuration is included.
- Validate the included SQL seed data and review upload/security behavior before using with real users.

## 👤 Author

**Brian Dol**, Senior Full Stack Engineer · [Portfolio](https://portfolio.dol-brian23.workers.dev/) · [LinkedIn](https://linkedin.com/in/brian-dol-31a06115a/)
