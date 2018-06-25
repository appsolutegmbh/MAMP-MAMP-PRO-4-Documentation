---
title: MAMP PRO (Windows) Documentation > WordPress Troubleshooting
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### I am receiving an "Error establishing database connection" error.

Confirm your DB_NAME variable in your wp-config.php file corresponds to the database name in your MySQL database. Your wp-config.php file is located in your document root.

define('DB_NAME', 'wordpress');

---

Confirm your DB_USER in your wp-config.php file corresponds to your MySQL username. By default, MAMP PRO uses the MySQL 'root' user.

define('DB_USER', 'root');

---

Confirm your DB_PASSWORD in you wp-config.php files corresponds to your MySQL database password. By default, MAMP PRO uses 'root' as the password for the MySQL 'root' user. Your password can be changed on the MySQL tab.

define('DB_PASSWORD', 'root');

---

Confirm your DB_Host includes the MySQL port number.

define ('DB_HOST','localhost:8889');

or

define('DB_HOST','127.0.0.1:8889');
