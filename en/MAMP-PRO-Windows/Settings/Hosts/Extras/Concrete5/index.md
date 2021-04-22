---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > Extras > Concrete5
description: 
layout: default-2
product: MAMP PRO Windows
language: en
lastedit: 2021-03-26
---

## Settings > Hosts > Extras > Concrete5

Concrete5 is an open source content management system. More information about concrete5 can be found [here](https://www.concrete5.org){:target="_blank"}.

![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/Extras/Concrete5/ExtrasConcrete5.png)

*  **Name of the site:**  
   Name your site.

*  **Email address:**  
   Your email address.  
   
   <div class="alert" role="alert"> 
   Note: You must enter a valid email address to setup a concrete5 installation.
   </div>

*  **Directory:**  
   The installation directory. If it is left blank the concrete5 files will be copied directly to the document root folder.  
  
   <div class="alert" role="alert"> 
   Note: Do not install over a previous installation of concrete5! Files will be overwritten without warning. 
   </div>

*  **Database name:**  
   Set the name of your database schema which will be added to your local database.  
   After installation you can view this database for this instance of concrete5 using phpMyAdmin, Sequel Pro, or MySQLWorkbench. 
 
*  **User name:**  
   The concrete5 admin.
   <div class="alert" role="alert">
   Note: You will need this user name to login into your new of concrete5 site, please write this down. 
   </div>

*  **Password:**  
   The concrete5 admins default password.  
   <div class="alert" role="alert">   
   Note: You will need this password to login into your new concrete5 site, please write this down.
   </div>
   
---

### Configuration

If you choose to change the database port after installation, you must also change the port number in the "application\config\database.php" file in your document root. Your port number is part of the "server" variable.