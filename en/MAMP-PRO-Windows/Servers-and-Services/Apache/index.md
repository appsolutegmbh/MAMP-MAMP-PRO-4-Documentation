---
title: MAMP PRO (Mac) Documentation > Servers and Services > Apache
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Servers and Services > Apache

The Apache Server is a popular web server used in production environments. An instance of Apache Server is installed on your Mac by MAMP PRO. Information on configuring your MAMP PRO Apache Server installation can be found [here](../../Settings/Hosts/Apache).

![MAMP](/en/MAMP-PRO-Windows/Servers-and-Services/Apache/Apache.png)

*  **Include Apache server in GroupStart**  

    Check to the Apache Server in the GroupStart. When activated Apache will automatically start/stop when the Servers button is pressed.

---

*  **Apache Modules**  

    The Apache Web Server installed by MAMP PRO comes with many modules pre-installed.

    The web server modules can be activated or deactivated depending on your needs. Module Description provides information pertaining to features and functions of the selected module.

    To enable the PHP scripting language you must activate the php_module, if you want to use Python you need mod_wsgi module, Perl needs perl_module. In order to switch to CGI mode and use multiple PHP versions you must activate cgi_module.

---

*  **Path To Apache log file**

    Errors occurring during execution of the Apache server will be saved in this log file.
