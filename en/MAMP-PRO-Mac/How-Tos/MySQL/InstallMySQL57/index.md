---
title: MAMP PRO (Mac) Documentation > How Tos > MySQL
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Upgrade MySQL to version 5.7

You cannot upgrade the MAMP PRO instance of MySQL. However you can install a separate instance of MySQL 5.7 on your Mac. 

<div class="alert" role="alert">
Note: We cannot provide support for installing or maintaining your MySQL 5.7 installation.
</div>

---

1. Download the [MySQL 5.7 Mac OS X 10.12 (x86, 64-bit), DMG Archive](https://dev.mysql.com/downloads/mysql/5.7.html){:target="_blank"}, or latest MySQL 5.7 release. 

2. Complete the installation of MySQL 5.7.

3. Start your MySQL 5.7 server in System Preferences.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/MySQL/InstallMySQL57/MySQLRunning.png)

Once you have successfully installed MAMP PRO you can run both instances of MySQL, or just your new MySQL 5.7. You must run your MySQL installations on different ports if you run both simultaneously.

---

#### MySQL 5.7 data default location

The default location for your database data is `/usr/local/mysql/data`.

---

#### Install Wordpress with MySQL 5.7

Create an empty database in MySQL, this example uses the default name "wordpress". Confirm you are using port 3306 to connect to MySQL.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/MySQL/InstallMySQL57/wordpressInstallation.png)

---

#### Connect to MySQL 5.7 using PHP

{% highlight php %}

$user = 'root';
$password = 'root';
$db = 'inventory';
$host = '127.0.0.1';
$port = 3306;

$link = mysqli_init();
$success = mysqli_real_connect(
   $link, 
   $host, 
   $user, 
   $password, 
   $db,
   $port
);

{% endhighlight %}










