---
title: MAMP PRO (Mac) Documentation > Servers and Services > Nginx
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Servers and Services > Nginx

The Nginx Web Server is a popular web server used in production environments. An instance of Nginx is installed on your Mac by MAMP PRO.  Information on how to custom configure your Nginx Server can be found [here](../../Settings/Hosts/Nginx) . 

![MAMP](/en/MAMP-PRO-Mac/Servers-and-Services/Nginx/Nginx.png)

*  **Include Nginx server in GroupStart**  

    Check to include the Nginx Server in GroupStart. When activated Nginx will automatically start/stop when the Servers button is pressed.

---

*  **Use Nginx as a Reverse Proxy for Apache**  

    Check to use Nginx as a reverse proxy for Apache. When this option is checked the following will be added to your  `/Library/Application Support/appsolute/MAMP PRO/conf/nginx.conf` file. Your requests will now be forwarded to your Apache server localhost.
    
    {% highlight php %}
        # proxy the PHP scripts to Apache
        location ~ \.php$ {
            proxy_set_header Host $host;
            proxy_set_header X-Real-IP $remote_addr;
            proxy_pass http://xxx.xxx.x.xxx:8888;
        }    
    {% endhighlight %}

It is possible to set your reverse proxy to forward php scripts to a [host other than localhost](../../How-Tos/General#nginx_reverse_proxy).

---

*  **Nginx Modules**

    The Nginx Web Server installed by MAMP PRO comes with several modules pre-installed.

    The web server modules can be activated or deactivated depending on your needs. Module Description provides information pertaining to features and functions of the selected module.

---

*  **Path to Nginx log file**

    Errors occurring during execution of the Nginx server will be saved in this log file.
