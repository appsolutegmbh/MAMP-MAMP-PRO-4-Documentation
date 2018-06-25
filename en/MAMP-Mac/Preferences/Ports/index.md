---
title: MAMP (Mac) Documentation > Preferences > Ports
description: MAMP (Mac) Documentation > Preferences > Ports
layout: default-2
product: MAMP Mac
language: en
---

## Preferences > Ports

![MAMP](/en/MAMP-Mac/Preferences/Ports/Ports.png)

Server programs, when addressed via the network, need to be assigned to a certain network port. This way, multiple server programs may run on one server machine. Every service has a default port: The Apache web server typically uses port 80, the MySQL database server utilises port 3306.

These ports are configurable. The default configuration for MAMP uses ports 8888 and 8889, and 7888. That way, the MAMP servers can run alongside other servers installed on your Mac. Should ports 7888, 8888 or 8889 be in use by a different application, please change the values accordingly.

The button Set Web & MySQL ports to 80 & 3306 will set the ports to the value commonly used on the internet. The button Set MAMP ports to default will reset the ports for Apache, Nginx and MySQL to 8888, 7888 and 8889.

If you want MAMP to be available via the Internet please make sure that the configured ports are opened in your firewall.
