---
title: MAMP PRO (Mac) Documentation > Menu > File
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

##  Menu > File

### Edit Template:<a name="edit_templates"></a>

MAMP PRO uses templates to create the necessary server config files. You can edit these templates from the menu item       File > Edit Template. Here, you have access to options which are not accessible from the MAMP PRO user interface.

A template file is created in `~/Library/Application Support/appsolute/MAMP PRO/templates` when you make a change to one     of your templates. There are separate templates for your Apache, Apache SSL, Nginx, PHP, and MySQL configurations. If you have not made any changes to your templates, your `~/Library/Application Support/appsolute/MAMP PRO/templates` directory will be empty.
     
<div class="alert" role="alert">
Note: Errors in the templates files can cause servers not to start. You should edit these templates only if you are familiar with the exact syntax and meaning of the options.
</div>
 
*  **Apache (httpd.conf and httpd-ssl.conf)**     
   
     Open and edit your httd.conf template file here. Changes made to your template file will be reflected your real      httpd.conf file. The httpd.conf file created from the template file and is located in `/Library/Application Support/appsolute/MAMP PRO/conf`. You can check this file to verify changes you are making in your template file are properly reflected.

     <div class="alert" role="alert">
     Changes are reflected in your real httpd.conf file after your servers are restarted. This applies to all           configuration files including nginx.conf, php.ini, my.cnf and main.cnf.
     </div>

*  **Nginx (nginx.conf)**   

     Open and edit your nginx.conf template file here. Changes made to your template file will be reflected your        real nginx.conf file. The nginx.conf file created from the template file and is located in `/Library/Application Support/appsolute/MAMP PRO/conf`.

*  **PHP (php.ini)**        
     
     Open and edit your php.ini template file here. There are likely several versions of php available, each of them with  their own template file. Changes made to your template file will be reflected your real php.ini file. The php.ini file created from the template file and is located in `/Library/Application Support/appsolute/MAMP PRO/conf`.
     
     ![MAMP](/en/MAMP-PRO-Mac/Menu/File/PHPini.png)

*  **MySQL(my.cnf)**        
     
     Open and edit your my.cnf template file here. There are likely several versions of MySQL available, each of them with their own template file. Changes made to your template file will be reflected your real my.cnf file. The my.cnf file created from the template file and is located in `/Library/Application Support/appsolute/MAMP PRO/conf`.
 
*  **Postfix (main.cf)** 
     
     Open and edit your main.cnf template file here. There are likely several versions of MySQL available, each of them with their own template file. Changes made to your template file will be reflected your real main.cnf file. The main.cnf file created from the template file and is located in `/Library/Application Support/appsolute/MAMP PRO/conf`.
 


<i class="fa fa-play-circle-o fa-lg" aria-hidden="true"></i>  [MAMP PRO and httpd.conf,nginx.conf php.ini, my.cnf](https://www.youtube.com/watch?v=tYLykP2CxMM){:target="_blank"}

---

### Export Template:
     
Export your current templates.

### Import Template:    

Import external templates.
     
<div class="alert" role="alert">
Importing templates made in a different version of MAMP PRO may cause some configuration files to be invalid thus preventing servers from being started.
</div>

---

### Factory Settings:
  
*  **Setting 1**     

     Setting 1 will reset all your host and server settings back to default, including setting your Apache ports back to 8888, 8890, 8889, and your Apache User/MySQL User to username/username.

*  **Setting 2**    

     Setting 2 will reset all your host and server settings back to default, including setting your ports back to 80, 440, 3306, and your Apache User/MySQL User to www/mysql.

<a name="backup"></a> 

---

### Backup…:

Make a backup of all your host settings, host and database files.

![MAMP](/en/MAMP-PRO-Mac/Menu/File/Backup.png)
     
### Restore From Backup:

Restore files from a previous backup.

![MAMP](/en/MAMP-PRO-Mac/Menu/File/Restore.png)

<div class="alert" role="alert">
Note: Restoring your backed up files can potentially overwrite your current host and database files. Back up your current host and database files before restoring from a backup. 
</div>




