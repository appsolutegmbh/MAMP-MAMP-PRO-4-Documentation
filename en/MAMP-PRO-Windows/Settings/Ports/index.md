---
title: MAMP PRO (Windows) Documentation > Settings > Ports
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Settings > Ports

Server programs, when addressed via the network, need to be assigned to a certain network port. This way, multiple server programs may run on one server machine. Every service has a default port: The Apache web server typically uses port 80, the MySQL database server utilises port 3306.

These ports are configurable. The default configuration for MAMP PRO uses ports 8888, 8889 and 8890. That way, the MAMP servers can run alongside other servers installed on your PC. Should ports 8888, 8889 or 8890 be in use by a different application, please change the values accordingly.

![MAMP](/en/MAMP-PRO-Windows/Settings/Ports/Ports.png)

*  **Set ports to 80, 81, 443, 7443 and 3306**  
   Set the ports to the value commonly used on the internet.
   
*  **Set default MAMP ports**  
   Set the ports for Apache, Nginx and MySQL to 8888, 8889 and 8890.
   
*  **Having trouble with blocked ports?**  
   MAMP PRO will auto detect free ports to use.

*  **Start Groupstart servers at system start**  
   Apache, Nginx and MySQL are started during startup of the OS, this means that the services are available before a user
   has logged into the system.

*  **Start Groupstart servers at startup of MAMP PRO**  
   The services will start automatically at startup of MAMP PRO.

*  **Stop Groupstart servers at shutdown of MAMP PRO**  
   The services will be stopped automatically when MAMP PRO shuts down.

*  **Delete log files at server startup**  
   The log files will be emptied before startup of the services. That way only current entries will be in the log files.
