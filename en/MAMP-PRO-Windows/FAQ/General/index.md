---
title: MAMP PRO (Windows) Documentation > FAQ > General
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## FAQ - General


### Are updates free of charge?

Yes, all updates in the current major version (4.x) are free of charge. To update MAMP PRO from e.g. 4.1.2 to 4.9 just use the serial number you already have. Licenses are good forever, they are not on a subscription basis. MAMP PRO 3 Windows licenses are also valid for MAMP PRO 4 Windows.

---

### Is MAMP PRO compatible with Windows 10?

Yes, MAMP PRO is compatible with Windows 10.

---

### Can I use MAMP at the same time as MAMP PRO?

Both applications, MAMP as well as MAMP PRO, are configuration tools for the tools inside the folder MAMP. Though you could run them simultaneously you should not. You may run into sporadic problems, even data loss can occur.

---

### Is it possible to add an updated version of PHP?

You can add additional PHP versions through the user interface.  More information on how to do this can  be  found [here](../../Languages/PHP).

---

### Is the ImageMagick PHP module included?

The ImageMagick PHP module is included by default, but you must enable it using the [PHP tab](../../Languages/PHP) in MAMP PRO. 

---

### Which Apache modules are included?

Apache modules are located in the `C:\MAMP\Library\modules` folder.

---

### Where can I find the log files?

Your log files are located in `C:\MAMP\logs`. You can access the various logs through the MAMP PRO interface.

---

### Will MAMP work if the MAMP folder is not located in the C:\ directory?

Yes it can be installed on any drive which is registered in Windows system. But because of simplicity, security and user permissions we always adwise installing on default  `C:\` drive.

---

### Are the amount of virtual hosts aliases limited?

No, with MAMP PRO you can use as many hosts and aliases as you like.

---

### Where exactly are the MAMP PRO files created or changed?

The following list contains all files which are created and changed by MAMP PRO and are not located within the MAMP PRO folder.

*  **MAMP PRO Settings and Files**  
   `C:\Users\Public\Documents\Appsolute\MAMPPRO\`
   `C:\Users\Public\Documents\Appsolute\MAMPPRO\conf\`
   `C:\Users\[MyUserName]\AppData\Roaming\Appsolute\MAMPPRO\userdb\`

   Please just change [MyUserName] to your username.

---

### Where are the configuration files located?

The changes you make in the MAMP PRO interface and template files help create real configuration files. The configuration files are recreated every time you start your servers. You cannot edit these files directly, however you can view them to verify your changes in the interface or template files are correctly being reflected.

*  **PHP**  
 `C:\Users\Public\Public Documents\Appsolute\MAMPPRO\conf\php.ini`

*  **MySQL**  
 `C:\Users\Public\Public Documents\Appsolute\MAMPPRO\conf\my.ini`

*  **Apache**  
 `C:\Users\Public\Public Documents\Appsolute\MAMPPRO\conf\httpd.conf`

*  **Apache-SSL**  
 `C:\Users\Public\Public Documents\Appsolute\MAMPPRO\conf\httpd-ssl.conf`

*  **Nginx**  
 `C:\Users\Public\Public Documents\Appsolute\MAMPPRO\conf\nginx.conf`

---

### Where can I find more information on the various servers, interpreters, debuggers and other tools that MAMP PRO uses?

Click on the following links for further information on

*  **Servers & Services**  

   [Apache Server](https://httpd.apache.org){:target="_blank"}
  
   [Nginx Server](https://httpd.apache.org){:target="_blank"}

   [MySQL](https://www.mysql.com){:target="_blank"}

*  **Languages**  

   [PHP](http://php.net){:target="_blank"}

   [Ruby](http://www.ruby-lang.org/en/){:target="_blank"}

   [Perl](https://www.perl.org){:target="_blank"}

   [Python](https://www.python.org){:target="_blank"}
   
*  **Cache Options & Debugger**   
  
   [MacGDP](http://www.bluestatic.org/software/macgdbp/){:target="_blank"}

   [APC](http://php.net/manual/en/book.apc.php){:target="_blank"}

   [eaccelerator](http://eaccelerator.net){:target="_blank"}

   [xcache](https://xcache.lighttpd.net){:target="_blank"}

   [opcache](http://php.net/manual/en/book.opcache.php){:target="_blank"}
   
*  **Database Administration**   

   [phpMyAdmin](https://www.phpmyadmin.net){:target="_blank"}

   [Sequel Pro](http://www.sequelpro.com){:target="_blank"}

   [MySQL Workbench](http://mysqlworkbench.org){:target="_blank"}
   
*  **Content Management Systems** 

   [WordPress](https://wordpress.org){:target="_blank"}
   
   [Joomla](https://www.joomla.org){:target="_blank"}
   
   [Drupal](https://www.drupal.org){:target="_blank"}
   
   [webEdition](http://www.webedition.org){:target="_blank"}
   
   [Magento](https://magento.com){:target="_blank"}
   
   [Mediawiki](https://www.mediawiki.org/wiki/MediaWiki){:target="_blank"}
   
   [phpBB](https://www.phpbb.com){:target="_blank"}
   
   [PrestaShop](https://www.prestashop.com){:target="_blank"}
   
   
*  **Dyn DNS Providers**
   
   [DNS-O-Matic](https://dnsomatic.com){:target="_blank"} 
   
   [no-ip](https://no-ip.com){:target="_blank"}    
   
   [dyn](https://dyn.com){:target="_blank"} 
   
   [easydns](https://easydns.com){:target="_blank"}
   
   


