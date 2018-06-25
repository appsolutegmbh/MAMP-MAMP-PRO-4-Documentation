---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > Extras > phpBB
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Settings > Hosts > Extras > phpBB

phpBB is an Internet forum package written in the PHP scripting language. More information about phpBB can be found [here](https://www.phpbb.com){:target="_blank"}.

![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/phpBB/phpBB.png)

*  **Email address:**  
   Your email address. You phpBB installation will send error messages to this e-mail address.
   <div class="alert" role="alert">   
   Note: You must enter a valid email address to setup a phpBB installation.
   </div>

*  **Directory:**  
   The installation directory. If it is left blank the phpBB files will be copied directly to the document root folder. If you provide a name, a subdirectoy will be created and your phpBB files will be placed in this directory.  
   <div class="alert" role="alert">
   Note: Do not install over a previous installation of phpBB! Files will be overwritten without warning.
   </div>

*  **Table Prefix:**  
   phpBB can use a table prefix to manage multiple forums in a single database. 

*  **Database name:**  
   Set the name of your database schema which will be added to your local database.  
   After installation you can view this database using phpMyAdmin, Sequel Pro, or MySQLWorkbench. 
 
*  **Username:**  
   The phpBB admin. Use this username to log into the admin area of your phpBB installation. 
   <div class="alert" role="alert">   
   Note: You will need this username to login into your new of phpBB installation, please write this down.
   </div>
*  **Password:**  
   The phpBB admins default password. Use this password to log into the admin area of your phpBB installation.
   <div class="alert" role="alert">
   Note: You will need this password to login into your new phpBB installation, please write this down.
   </div>
   
   ---

### Installation
 
After your phpBB extra is installed you will see two links to your site. The ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/BlackArrow.png) button will open your Extra's homepage. The ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/gear.png) button will open the admin page of your phpBB site. Your admin page is in the `ucp.php` file in your document root. Your database name is indicated to the right of the  ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/mysql.png) icon, your database table prefix is in parenthesis.

![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/phpBB/installphpBB.png)


