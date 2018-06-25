---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > Extras > Magento
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Settings > Hosts > Extras > Magento

Magento Commerce is a popular php based e-commerce platform. More information about Magento can be found [here](https://www.magento.com){:target="_blank"}.

![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/Magento/Magento.png)

*  **Email address:**  
   Your email address. Your Magento installation will send error messages to this email address.
   <div class="alert" role="alert">   
   Note: You must enter a valid email address to setup a Magento installation.
   </div>

*  **Directory:**  
   If you would like to install Magento directly in the host document root directory, leave this field empty. If you provide a name, Magento will be installed in this directory. The directory must not yet exist.  
   
   <div class="alert" role="alert">      
   Note: Do not install over a previous installation of Magento! Files will be overwritten without warning.
   </div>

*  **Table Prefix:**  
   Magento can use a table prefix to manage multiple web sites in a single database. The prefix has a maximum of five characters.

*  **Database Name:**  
   Set the name of your database schema. After installation you can view this database using phpMyAdmin, Sequel Pro, or MySQLWorkbench.
 
*  **Username:**  
   Use this username to login into the Magento adminn area.  
   <div class="alert" role="alert">   
   Note: You will need this username to login into your new of Magento e-commerce site, please write this down. 
   </div>

*  **Password:**  
   Use this Magento password to login to the admin area of your installation.  
   <div class="alert" role="alert">   
   Note: You will need this password to login into your new Magento e-commerce site, please write this down.
   </div>

*  **Encryption Key:**  
   This key is used for encrypting your sensitive data. You will need it if you move your data to a different Magento installation. Some payment and shipment processors require it. The key is located in <document root>/app/etc/env.php .

---

### Installation
 
After your Magento extra is installed you will see two links to your site. The ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/BlackArrow.png) button will open your Extra's homepage. The ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/gear.png) button will open the admin page of your Magento site. Your database name is indicated to the right of the  ![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/mysql.png) icon, your database table prefix is in parenthesis.

![MAMP](/en/MAMP-PRO-Mac/Settings/Hosts/Extras/Magento/installMagento.png)
