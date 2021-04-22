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

![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/Extras/Joomla/ExtraJoomla.png)

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
   
*  **User name:**  
   The Joomla admin's name.
   <div class="alert" role="alert">
   Note: You will need this user name to login into your new of Joomla site, please write this down. 
   </div>

*  **Password:**  
   The Joomla admin's default password.  
   <div class="alert" role="alert">   
   Note: You will need this password to login into your new Joomla site, please write this down.
   </div>
   
---
 
### Configuration

Your Joomla Extra is configured in the configuration.php file in the document root folder. If you choose to change the database port after installation, you must also change the port number in the "$host" variable.

