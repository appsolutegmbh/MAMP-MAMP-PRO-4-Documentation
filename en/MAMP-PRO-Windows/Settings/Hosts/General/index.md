---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > General
description: 
layout: default-2
product: MAMP PRO Windows
language: en
lastedit: 2021-03-26
---

## Settings > Hosts > General

MAMP PRO uses virtual hosts to allow your web servers to serve different websites. The virtual host "localhost" is created by default and cannot be deleted. You can add an unlimited number of hosts allowing you to create one host per project. Every host can have it's own directory to store html, PHP files, and images. This directory is called Document Root.

The name of a host (server name) must be unique, often it's practical to use a reverse domain naming scheme to easily identify them (e.g. use info.mamp.development instead of development.mamp.info). The unreversed name may conflict with an outside domain name.

To create a new host press the "Plus" button at the bottom left of the hosts table.

![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/General/OpenHost.png)

*  **Host name**

   The server name and port number in combination must be unique within MAMP PRO. The host name may only contain letters and/or numbers, as well as dashes ("-"); but it may not begin or end with a "-" character. Names are not case-sensitive (upper and lower-case letters are not distinguished.)

*  **Document root**

   The location of the documents (HTML/PHP files etc.) of a virtual host is called a document root. The document root is also known as the web root folder. MAMP PRO will automatically add an "index.php" file and a MAMP image to this location when your web server is restarted if the folder is empty. 

---

*  **Create a database named**

   You can optionally create a MySQL database. Most content management systems require a database, and you can conveniently add one here.

*  **Copy the contents of a template folder to the document root**

   You can optionally add the contents of a templates folder. You may use the same template, js, and css files/folders in every site you develop. Use this option to copy the contents of your template folder to your new document root folder.

---

![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/General/General.png)

*  **Hosts Table**

   The hosts table contains five columns. The first column contains your host name. The second column indicates which web server will host the file. 

   The third column indicates whether the host is active. If left unchecked, the host will not be active and cannot be viewed in a web browser.

   The fourth column contains the PHP version that is used with host. The fifth column will display an icon of the Extra installed if an Extra is installed.

---

<a name="open_host"></a>

*  **Hostname**  
   The server name and port number in combination must be unique within MAMP PRO.
   The host name may only contain letters and/or numbers, as well as dashes ("-");
   but it may not begin or end with a "-" character.
   Names are not case-sensitive.

   If the servers are running you can use the Open button to open a host in your web browser.

*  **IP address**  
   If this field is left empty or contains an `*` the web server will use one of the computer's IP addresses to access this host. If you want to choose which of the IP addresses should be associated with a host, then select it from the pop up menu.

*  **Port number**  
   Determine the port with which the virtual host is accessible. Valid values are from 1 to 65535.
   In most cases the preset value does not need to be changed.

<a name="setting_php_version"></a> 

*  **PHP Version**  
   Determine which version of PHP a host will use. This can only be set when Individual PHP version
   for every host (CGI) is set in the PHP section of MAMP PRO.

   If you select the default PHP version MAMP PRO will automatically adapt this setting if you choose
   a new default version in the PHP tab. Use a fixed setting to tell MAMP PRO not to alter the PHP version.
   
      ![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/General/phpVersions.png)

   Sounds complicated? Let's take a look at an example: The default version is set to 5.5.9. You have oneHost
   set to PHP version "Default (5.5.9)", anotherHost set to "5.5.9" and yetAnotherHost set to "5.3.28".
   If you set the PHP version in the PHP section to "5.4.25", MAMP PRO will adapt the PHP version of oneHost to this version (it is set to always use the standard version). The other 2 hosts will not be changed.
  
     <a name="php_info_access_button"></a> 

      *  **PHPInfo**
      
         ![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/General/phpInfoLink.png)
      
         View your PHP configuration by pressing the "i" button to the right of the version name.
      
*  **Dynamic DNS**  
   Determines, if this virtual host is accessible with the Dynamic DNS service from the internet.

*  **Use with server**  
    Determine which web server will be used with your host. An icon next to the server name in the server list will also indicate which web server you chose.

---

<a name="mamp_viewer"></a> 

*  **Name resolution**  
   This will determine how your system will map host names to ip addresses.

    *  **via hosts file**  
       The basic mapping mechanism which uses the the file "C:\Windows\System32\drivers\etc\hosts".
       
    *  **for "MAMP Viewer" (LAN only)**  
       Enable your host to be viewed on the MAMP Viewer.

    *  **via Xip.io (LAN only)**  
       Allow other computers on your local network to access your web site. Using the Share button you can send the Xip.io address to other users.
      
         <div class="alert" role="alert">
         Note: The Xip.io addresses will only work in your local network. They are temporary and may become invalid if you restart your PC. Also make sure that your Internet router is not blocking Xip.io calls by using a DNS Rebind protection. If the router does this you can either deactivate this function, add Xip.io as an exception or not use the router as DNS Server in your PCs network settings.
         </div>

*  **Document root**  
   The location of the documents (HTML/PHP files etc.) of a virtual host is called a document root.

*  **Alias Name**  
   Aliases are additional names for your virtual host. The same constraints apply to these additional names as to the host itself. Add aliases with the plus-button.
   
   ---
   
   To remove a new host press the "Minus" button at the bottom left of the screen.
   
   ![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/General/removeHost.png)
   
   *  **Delete document root folder**
   
      MAMP PRO will delete your document root folder and all of its contents.
   
   *  **Remove the databases of the installed Extras**
   
      If your host is an Extra, MAMP PRO will delete the database installed Extra database.