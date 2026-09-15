# Inventory Management System

A browser-based inventory management application built with **PHP, MySQL, JavaScript, HTML, and CSS**. The project provides a simple CRUD workflow for maintaining inventory records through a local XAMPP-style PHP/MySQL environment.

## Overview

The application demonstrates a traditional server-rendered web stack: PHP handles requests and database operations, MySQL stores inventory data, and the frontend provides forms and views for managing items.

The repository includes the application source, SQL/database backup files, styles/assets, and dedicated scripts for adding, editing, and deleting inventory records.

## Core functionality

- View inventory records from the main application page
- Add new inventory items
- Edit existing records
- Delete records
- Connect PHP to a MySQL database
- Restore/create the project database from the included SQL files
- Run locally through Apache and MySQL

## Architecture

```text
Browser
   │
   ▼
PHP application
   ├── index.php      → main inventory view
   ├── additem.php    → create records
   ├── edit.php       → update records
   ├── delete.php     → remove records
   └── config.php     → database connection
          │
          ▼
       MySQL
```

## Repository structure

```text
Inventory-Management-/
├── index.php
├── additem.php
├── edit.php
├── delete.php
├── config.php
├── errors.php
├── inventorymanagement.sql
├── Database_backup/
├── assets/
├── css/
├── fonts/
├── images/
├── image.jpg
└── README.md
```

## Local setup

### 1. Install a PHP/MySQL environment

The original project was designed to run locally with **XAMPP**. Start:

- Apache
- MySQL

### 2. Place the project in the web root

For a standard XAMPP installation, copy/clone the project under `htdocs`:

```text
C:/xampp/htdocs/Inventory-Management-/
```

### 3. Create the database

Open phpMyAdmin and import:

```text
inventorymanagement.sql
```

A database backup directory is also included in the repository.

### 4. Configure the connection

Review `config.php` and make sure its MySQL host, username, password, and database values match your local environment.

### 5. Open the application

With Apache and MySQL running, visit the corresponding localhost path, for example:

```text
http://localhost/Inventory-Management-/
```

## Tech stack

| Layer | Technology |
|---|---|
| Backend | PHP |
| Database | MySQL |
| Frontend | HTML, CSS, JavaScript |
| Local server | Apache / XAMPP |
| Database tooling | MySQL Workbench / phpMyAdmin-compatible SQL |

## What this project demonstrates

- CRUD application design
- PHP-to-MySQL connectivity
- SQL-backed web forms
- Server-side request handling
- Separation of create/update/delete operations
- Local web-server deployment

## Limitations

This is an academic/learning project and reflects a traditional PHP application structure. Before using a similar design in production, it should be reviewed for modern security practices such as parameterized queries, stronger validation, authentication/authorization, CSRF protection, secret management, and production-ready error handling.

## Possible improvements

- Replace raw database queries with prepared statements
- Add authentication and role-based access control
- Add search, filters, sorting, and pagination
- Add stock-level alerts and transaction history
- Move configuration to environment variables
- Add automated tests
- Reorganize the project into a clearer MVC-style structure
- Containerize the app with Docker for reproducible setup

---

This repository is preserved as a full-stack inventory-management project demonstrating CRUD operations with PHP and MySQL.
