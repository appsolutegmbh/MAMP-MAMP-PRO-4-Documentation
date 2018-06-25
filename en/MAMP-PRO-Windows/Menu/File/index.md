---
title: MAMP PRO (Windows) Documentation > Menu > File
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

##  Menu > File

### Edit Template:<a name="edit_templates"></a>

MAMP PRO uses templates to create the necessary server config files. You can edit these templates from the menu item       File > Edit template. Here, you have access to options which are not accessible from the MAMP PRO user interface.

A template file is created in `C:\Users\[username]\AppData\Roaming\Appsolute\MAMPPRO\templates` when you make a change to one of your templates. There are separate templates for your Apache, Apache SSL, Nginx PHP, and MySQL configurations.
     
<div class="alert" role="alert">
Note: Errors in the templates of the configuration files can cause the servers not to start. You should edit these templates only if you are familiar with the exact syntax and meaning of the options.
</div>
 
*  **Apache (httpd.conf and httpd-ssl.conf)**     
   
     Open and edit your httd.conf template file here. Changes made to your template file will be reflected your         real      httpd.conf file. The httpd.conf file created from the template file and is located in `C:\Users\Public\Documents\Appsolute\MAMPPRO\conf\`. You can check this file to verify changes you are making in your template file are properly reflected.

     <div class="alert" role="alert">
     Changes are reflected in your real httpd.conf file after your servers are restarted. This applies to all           configuration files including nginx.conf, php.ini, my.cnf and main.cnf.
     </div>

*  **Nginx (nginx.conf)**   

     Open and edit your nginx.conf template file here. Changes made to your template file will be reflected your        real nginx.conf file. The nginx.conf file created from the template file and is located in `C:\Users\Public\Documents\Appsolute\MAMPPRO\conf\`.

*  **PHP (php.ini)**        
     
     Open and edit your php.ini template file here. There are likely several versions of php available, each of them with  their own template file. Changes made to your template file will be reflected your real php.ini file. The php.ini file created from the template file and is located in `C:\Users\Public\Documents\Appsolute\MAMPPRO\conf\`.
     
     ![MAMP](/en/MAMP-PRO-Windows/Menu/File/PHPini.png)

*  **MySQL(my.cnf)**        
     
     Open and edit your my.cnf template file here. There are likely several versions of MySQL available, each of them with their own template file. Changes made to your template file will be reflected your real my.cnf file. The my.cnf file created from the template file and is located in `C:\Users\Public\Documents\Appsolute\MAMPPRO\conf\`.
 
### Factory Settings:
  
*  **Development**     

     Setting 1 will reset all your host and server settings back to default, including setting your Apache ports back to 8888, 8890, 8889, and your Apache User/MySQL User to username/username.


<a name="backup"></a> 

---

### Backup…:

Make a backup of all your host settings, host and database files.

![MAMP](/en/MAMP-PRO-Windows/Menu/File/Backup.png)
     
### Restore From Backup:

Restore files from a previous backup.

![MAMP](/en/MAMP-PRO-Windows/Menu/File/Restore.png)

<div class="alert" role="alert">
Note: Restoring your backed up files can potentially overwrite your current host and database files. Back up your current host and database files before restoring from a backup. 
</div>

---

### Settings

 ![MAMP](/en/MAMP-PRO-Windows/Menu/File/Settings.png)
 
 
 *  **Open Webstart When starting MAMP PRO**
 
     Check this box to open a browser to the Webstart page when you start MAMP PRO. 
 
 *  **Path to Webstart:**
 
     The path set to your Webstart page. This is by default, using an Alias, set to [http://localhost:8888/MAMP](http://localhost:8888/MAMP).
 
 *  **Allow Saving**
 
     Allow saving when MAMP PRO detects an invalid document root or IP Address.
 
 *  **Apache and MySQL servers start as:**
 
     MAMP PRO can run Apache and MySQL as a service or a process. Apache and MySQL on Windows are set to service as          default for MAMP PRO Windows installation. When servers runs under "Network service" it is more security restricted then when servers run as processes under the current user.
     
     
 


