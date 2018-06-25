---
title: MAMP PRO (Mac) Documentation > Servers and Services > MySQL
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Servers and Services > MySQL

The MySQL database server is a popular database used on production servers. An installation of MySQL is installed on your computer by MAMP PRO. Your MAMP PRO MySQL database data is located in `/Library/Application Support/appsolute/MAMP PRO/db/mysql56`.

<i class="fa fa-play-circle-o fa-lg" aria-hidden="true"></i>  [MAMP PRO MySQL Data](https://www.youtube.com/watch?v=ZRHJy2K4yzc){:target="_blank"}

![MAMP](/en/MAMP-PRO-Mac/Servers-and-Services/MySQL/MySQL.png)

*  **Include MySQL server in GroupStart**  
   Check to include the MySQL Server in the GroupStart. When activated MySQL server will automatically start/stop when the Servers button is pressed.

---

*  **Version**  
   The current MySQL version.

*  **Data directory**  
   Displays the location of your MySQL Data. This location cannot be changed.
   <div class="alert" role="alert">
   The MAMP PRO Uninstaller will delete this directory. Make backups before using the uninstller!
   </div>

---

*  **Change password of user "root"**  
   The Head Database Administrator is called root. This user has unlimited access to all databases.
   Therefore you should set the password to one only you know.  
   
   <div class="alert" role="alert"> 
   Note: The default password of root is "root". To make things even more confusing there is also a user root inside Mac        OS X. Don't confuse them. You can also use one of the MySQL administration tools to create other MySQL users if you do not    want to use almighty root.*
   </div>

---

*  **Allow network access to MySQL**  
   If the checkbox for allow network access to MySQL is not checked, network access to the database is prohibited,
   even from programs installed locally.

   <div class="alert" role="alert"> 
   Note: This is an advanced feature not needed for local development.
   </div>
   
    *  **only from this Mac**  
       Only programs installed on this Mac can access MySQL via network functions.

    *  **from other computers**  
       MySQL will answer any network request, even from computers on the internet, depending on you network settings.

---

*  **Administer MySQL with**  
   MAMP PRO comes pre-installed with phpMyAdmin. You will see a direct link to both Sequel Pro and MySQL Workbench on the MySQL tab if you install them.

    *  **phpMyAdmin** is a web-based administrational tool. It allows you to change data and perform administrative duties
       like creating new databases.

    *  **Sequel Pro** is a native Mac application. It allows you to create and visualise database schemas in addition
       to administrative duties. More information on how to [connect to MySQL using Sequel Pro](../../How-Tos#connect_using_sequel_pro) can be found in our How To section.
       
      <i class="fa fa-play-circle-o fa-lg" aria-hidden="true"></i> [Using Sequel Pro With MAMP PRO](https://www.youtube.com/watch?v=MyNIr7XUpBI){:target="_blank"}

    *  **MySQLWorkbench** is also a native Mac application from the makers of MySQL. It allows you to visually create                 database schemas in addition to administrative duties.
    
    

---

*  **Path to MySQL log file**  
   Errors occurring at startup or during execution of the MySQL server will be saved in this log file.
