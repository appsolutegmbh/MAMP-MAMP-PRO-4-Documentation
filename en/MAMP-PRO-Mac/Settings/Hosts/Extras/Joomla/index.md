---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > Extras > Joomla
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Settings > Hosts > Extras > Joomla

Joomla is a free and open-source content management system. More information about Joomla can be found [here](https://www.joomla.org){:target="_blank"}.

Joomla installations can share a single MySQL database if you provide a unique table prefix during installation. To use an existing database enter the name of the database and a unique table prefix. To create a new database use a unique database name. The table prefix must not be empty.

![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/Joomla/Joomla.png)

*  **Name of the site:**  
   The name of your site.

*  **Email address:**  
   Your email address.  
   
   <div class="alert" role="alert"> 
   Note: You must enter a valid email address to setup a Joomla installation.
   </div>

*  **Directory:**  
   The installation directory. If it is left blank the Joomla files will be copied directly to the document root folder.  
  
   <div class="alert" role="alert"> 
   Note: Do not install over a previous installation of Joomla! Files will be overwritten without warning. 
   </div>

*  **Table prefix:**  
   Set the name of your database schema prefix. Joomla offers the ability to manage multiple websites using a single database schema.

*  **Database name:**  
   Set the name of your database schema which will be added to your local database.
   After installation you can view this database for this instance of Joomla using phpMyAdmin, Sequel Pro, or MySQLWorkbench.
   
*  **Username:**  
   The Joomla admin's name.
   <div class="alert" role="alert">
   Note: You will need this username to login into your new of Joomla site, please write this down. 
   </div>

*  **Password:**  
   The Joomla admin's default password.  
   <div class="alert" role="alert">   
   Note: You will need this password to login into your new Joomla site, please write this down.
   </div>
   
---
 
### Installation
 
After your Joomla extra is installed you will see two links to your site. The ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/BlackArrow.png) button will open your Extra's homepage. The ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/gear.png) button will open the admin page of your Joomla site. Your admin page is in the `/administrator` subdirectory of your document root. Your database name is indicated to the right of the  ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/mysql.png) icon, your database table prefix is in parenthesis.

![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/Joomla/joomlaInstall.png)



