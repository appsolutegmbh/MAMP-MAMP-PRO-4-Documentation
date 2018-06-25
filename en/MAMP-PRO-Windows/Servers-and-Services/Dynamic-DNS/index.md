---
title: MAMP PRO (Windows) Documentation > Servers and Services > Dynamic DNS
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Servers and Services > Dynamic DNS

If you would like to make your hosts accessible from the internet (Don't forget about security then!), but do not have a domain name that points to your PC, you will need a Dynamic DNS Service. 

If your network is connected to the internet via a router and it can handle Dynamic DNS Services, then you don’t need to configure it with MAMP PRO. 

Otherwise you will need to register with a Dynamic DNS Service and enter the username and password into the appropriate fields. Then you will need to tell MAMP PRO when to inform the Dynamic DNS provider about a change in your Macs IP address. It may be necessary when you restart your computer or a DSL/Cable modem re/establishes a connection.

<div class="alert" role="alert">
Note: To use the Dynamic DNS functions, you will need to register with one of the supported providers. This is independent of MAMP PRO and is not a service provided by appsolute GmbH.
</div>

![MAMP](/en/MAMP-PRO-Windows/Servers-and-Services/Dynamic-DNS/dynDNS.png)

---

*  **Include Dynamic DNS service in GroupStart**  
      Check to include the DNS Server in GroupStart. When activated the DNS Server will automatically start when the Servers button is pressed.

---

*  **Activate Service**  
    *  **Only while a web server is running**  
    *  **Permanently (as a System Service)**  

---

*  **Account data for service**

      Select the tab view of your dynamic dns service provider when you have an account with [DNS-O-Matic](https://dnsomatic.com){:target="_blank"}, [no-ip.com](https://no-ip.com){:target="_blank"},    [dyn.com](https://dyn.com){:target="_blank"}, or [easydns.com](https://easydns.com){:target="_blank"}. Select the Generic tab for all other dynamic dns service providers.

    *  **User name:**  
       Enter the user name that was given to you by the provider of the Dynamic DNS Service.  

    *  **Password:**  
       Enter the password that was given to you by the provider of the Dynamic DNS Service.
       
    *  **Server:**  
       Enter the server name ... .  

---

*  **Path to Dynamic DNS log file**  
      Events from the Dynamic DNS service will be recorded in a log file.
