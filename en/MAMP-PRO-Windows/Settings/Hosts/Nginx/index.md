---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > Nginx
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Settings > Hosts > Nginx

Nginx options can be set for the selected virtual host in the table. These options are security relevant!

<div class="alert" role="alert">
Note: You cannot make changes to the Nginx settings unless the host is set to Nginx on the Settings > Hosts > General tab.
</div>

![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/Nginx/Nginx.png)

*  **Directory index**  

   Determine which file Nginx should serve if no filename is given in an address. By default it is either index.html or index.php.
   
*  **AutoIndex**

   Activates or deactivates "directory browsing". If there is no index.html, index.php, etc in the document root, the content of the folder is displayed when this option is enabled. Without this option, nothing will be displayed or an error message will appear.
   
---
   
*  **Additional parameters for location:/**

   *  **try_files**
   
   *  **Custom**

---

*  **Access Limits**  

    *  **allow**
    
         Insert access limits here.
    
    *  **deny**
    
         Insert access deny limits here.
         
---
    
*  **Additional parameters for &lt;server&gt; directive**

   Add additional parameters to the &lt;server&gt; directive here.  

<div class="alert" role="alert">
Note: Watch out for typos, they will otherwise prevent Nginx from starting up.
</div>

---

*  **nginx.conf File**
   You cannot directly edit your nginx.conf file in MAMP PRO. You need to make custom configurations through your nginx.conf template file. More information on how to [configure your nginx template file](../../../Menu/File#edit_templates) can be found in our Menu > File section.

   <i class="fa fa-play-circle-o fa-lg" aria-hidden="true"></i> [MAMP PRO and httpd.conf, php.ini,                      my.cnf](https://www.youtube.com/watch?v=tYLykP2CxMM){:target="_blank"}


