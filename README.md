# **Secure Website with Role-Based Access Control (RBAC)**

## **Project Overview**
This project is a secure and responsive website built with PHP and MySQL, implementing **Authentication**, **Authorization**, and **Role-Based Access Control (RBAC)**. It includes the following features:

### **Features and Functionalities**:
- **User Authentication**:
  - Secure user registration and login.
  - Password hashing using PHP Data Objects (PDO).
  - Brute-force protection, session fixation prevention, and CSRF mitigation.

- **Role-Based Access Control (RBAC)**:
  - User roles: Admin, User, and Moderator.
  - Role-specific permissions for accessing and performing CRUD operations.

- **Secure Session Management**:
  - HttpOnly, Secure, and strict session cookies.
  - Session regeneration upon login to prevent fixation attacks.

- **Responsive Design**:
  - Designed using CSS Flexbox for mobile-first, responsive layouts.

- **Security Hardening**:
  - SQL injection, XSS, and CSRF prevention.
  - Apache and PHP configurations for enhanced server security.
  - HTTPS enforcement with SSL/TLS support.

---

## **System Requirements**
- **Operating System**: Windows/Linux/MacOS
- **Web Server**: Apache (e.g., XAMPP)
- **PHP Version**: PHP 7.4 or higher
- **Database**: MySQL
- **Browser**: Chrome, Firefox, or any modern web browser

---

## **Setup Instructions**

### **Step 1: Database Configuration**
1. Open the `db/` folder and locate the `secure_website.sql` file.
2. Import the SQL file into your MySQL server using your preferred database management tool (e.g., phpMyAdmin or MySQL Workbench).

### **Step 2: Copy Files to Server**
1. Copy all the content from the `src/` directory to your web server's root directory:
   - For **XAMPP**, copy it to `xampp/htdocs/`.
   - For **Linux**, place the files in `/var/www/html/`.

### **Step 3: Update Configuration**
1. Navigate to `src/php/config.ini` and update the database credentials:
   ```ini
   [database]
   host = "localhost"
   username = "root"
   password = ""
   dbname = "secure_website"
