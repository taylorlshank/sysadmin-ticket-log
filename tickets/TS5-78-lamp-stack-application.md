# TS5-78 – Install a LAMP Stack Application

## Overview
This ticket documents the deployment of a LAMP (Linux, Apache, MariaDB, PHP) stack and the installation of a CRM web application. The goal was to provision all required services, configure the database backend, and validate full application functionality through the web interface.

---

## Environment
- OS: Rocky Linux / RHEL 9
- Web Server: Apache (httpd)
- Database: MariaDB
- Scripting Language: PHP
- Application: CRM Web Application

---

## Tasks Performed

1. Updated the system and installed required LAMP packages  
2. Enabled and started Apache and MariaDB services  
3. Deployed CRM application files to the Apache web directory  
4. Created and configured the CRM database  
5. Installed PHP modules and phpMyAdmin  
6. Imported the CRM database schema  
7. Validated application access and user functionality  

---

## Validation

- Apache service running and serving web content
- PHP processing confirmed via info page
- Database connectivity verified
- CRM admin and user login functionality confirmed

---

## Screenshots

### 1. LAMP Services Installed and Running
![LAMP services installed](./assets/TS5-78/01-lamp-services-installed.png)
![LAMP services installed – continued](./assets/TS5-78/01-lamp-services-installed-02.png)
![LAMP services installed – continued](./assets/TS5-78/01-lamp-services-installed-03.png)

---

### 2. CRM Application Files Deployed
![CRM files deployed](./assets/TS5-78/02-crm-files-deployed.png)

---

### 3. CRM Database Created
![CRM database created](./assets/TS5-78/03-crm-database-created.png)

---

### 4. Database Connection Configured
![DB connection configured](./assets/TS5-78/04-dbconnection-configured-01.png)
![DB connection configured – continued](./assets/TS5-78/04-dbconnection-configured-02.png)

---

### 5. PHP Info Page Verified
![PHP info page](./assets/TS5-78/05-php-info-page-01.png)
![PHP info page – continued](./assets/TS5-78/05-php-info-page-02.png)

---

### 6. phpMyAdmin Access Verified
![phpMyAdmin access](./assets/TS5-78/06-phpmyadmin-access.png)

---

### 7. CRM Database Imported
![CRM database imported](./assets/TS5-78/07-crm-database-imported-01.png)
![CRM database imported – continued](./assets/TS5-78/07-crm-database-imported-02.png)

---

### 8. Admin Login Page Verified
![Admin login page](./assets/TS5-78/08-admin-login-page.png)

---

### 9. Admin Dashboard Accessed
![Admin dashboard](./assets/TS5-78/09-admin-dashboard.png)

---

### 10. User Login Successful
![User login success](./assets/TS5-78/10-user-login-success.png)


---

## What I Learned

- End-to-end deployment of a LAMP stack in an enterprise Linux environment
- Importance of correct file permissions and ownership for web applications
- Database-to-application connectivity troubleshooting
- Validating full-stack functionality beyond service-level checks
