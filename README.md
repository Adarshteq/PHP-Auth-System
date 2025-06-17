## PHP Auth System - Login & Register

A simple, clean, and responsive user authentication system built using PHP, HTML, CSS, and JavaScript. 

This project includes user registration, login, logout, session handling, and basic role-based redirection (admin and user pages).

## 🚀 Features

- 📝 User Registration with form validation

- 🔐 Secure Login system

- 👥 Role-based access: Admin and User

- 🔄 Session management with logout

- 🌐 Responsive frontend using modern CSS

- ⚠️ Error messages for failed login/register attempts

## 🛠️ Technologies Used

- **PHP** – Server-side logic

- **MySQL** – (Assumed for storing users)

- **HTML/CSS** – Frontend layout and styling

- **JavaScript** – Basic UI interactivity

- **Google Fonts (Poppins)** – Clean typography

## 📁 Folder Structure

php-auth-system-login-register/

├── index.php # Main page with login/register forms

├── login_register.php # Handles login and register actions

├── config.php # Database connection config

├── admin_page.php # Accessible by admin users only

├── user_page.php # Accessible by regular users only

├── logout.php # Ends session and logs user out

├── style.css # Styling for UI

├── script.js # Switch between login/register forms


## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Adarshteq/PHP-Auth-System-Login-Register.git
cd PHP-Auth-System-Login-Register
```

2. Set Up Local Server
  -Use XAMPP, WAMP, or MAMP.

  -Move the project folder to the htdocs directory.

3. Create MySQL Database

  -Open phpMyAdmin

  -Create a new database (e.g., auth_system)

  -Create a users table:

```sql
Copy
Edit
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL UNIQUE,
    password VARCHAR(255) NOT NULL,
    user_type VARCHAR(20) DEFAULT 'user'
);
```

4. Update config.php

  -Ensure the database credentials in config.php match your local setup:

```php
Copy
Edit
$conn = mysqli_connect('localhost', 'root', '', 'auth_system');
```

5. Run the Application

  -Open your browser and go to:

```pgsql
Copy
Edit
http://localhost/PHP-Auth-System-Login-Register/index.php
```
