---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > Extras > Wordpress
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Settings > Hosts > Extras > Wordpress

WordPress is a free and open-source content management system based on PHP and MySQL. More information about Wordpress can be found [here](https://www.wordpress.org){:target="_blank"}. You can find more information about your Wordpress installation in the Wordpress [documentation](https://codex.wordpress.org/Main_Page){:target="_blank"}.

<div class="alert" role="alert">
Note: When Wordpress is installed the host name and Apache port number are stored in its corresponding database. Changing the Apache port after installation will result in breaking your Wordpress installation. Port migration tools are available for Wordpress. It is generally advised to create Wordpress hosts using Apache port 80.
</div>


![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/WordPress/WordPress.png)

*  **Name of the blog:**  
   The name of your blog.

*  **Email address:**  
   Your email address.  
   <div class="alert" role="alert"> 
   Note: You must enter a valid email address to setup a WordPress installation.
   </div>

*  **Directory:**  
   The installation directory. If it is left blank the Wordpress files will be copied directly to the document root folder.  
   <div class="alert" role="alert">    
   Note: Do not install over a previous installation of Wordpress! Files will be overwritten without warning.  
   </div>

*  **Table prefix:**  
   Set the name of your database schema prefix. Wordpress offers the ability to manage multiple websites using a single database schema.

*  **Database name:**  
   Set the name of your database schema which will be added to your local database.  
   After installation you can view this database for this instance of WordPress using phpMyAdmin, Sequel Pro, or           MySQLWorkbench. 
 
*  **Username:**  
   The WordPress admin's username.
   <div class="alert" role="alert"> 
   Note: You will need this username to login into your new of WordPress blog, please write this down.
   </div>

*  **Password:**  
   The WordPress admin's default password.  
   <div class="alert" role="alert"> 
   Note: You will need this password to login into your new WordPress blog, please write this down.
   </div>

---
 
### Installation
 
After your WordPress extra is installed you will see two links to your site. The ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/BlackArrow.png) button will open your Extra's homepage. The ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/gear.png) button will open the admin page of your WordPress site. Your admin page is in `/wp-login.php` in your document root. Your database name is indicated to the right of the  ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/mysql.png) icon, your database table prefix is in parenthesis.

![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/WordPress/wpInstall.png)

---

### Configuration

Your Wordpress Extra is configured in the wp-config.php file in the document root folder.

---

### Videos

<i class="fa fa-play-circle-o fa-lg" aria-hidden="true"></i>  [Installing wordPress with Extras and Manually](https://www.youtube.com/watch?v=pZ7J4Ai-RxQ){:target="_blank"}

<i class="fa fa-play-circle-o fa-lg" aria-hidden="true"></i>  [Wordpress Multisite](https://www.youtube.com/watch?v=7pDvR9E94Og){:target="_blank"}






