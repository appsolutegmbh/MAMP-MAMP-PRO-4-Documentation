---
title: MAMP PRO (Mac) Documentation > How Tos > General > Accessing localhost on a LAN
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Accessing your MAMP PRO localhost on a LAN - local ip address or Local Hostname

You can access your MAMP PRO localhost on a LAN using mobile devices or other Macs.

<div class="alert" role="alert">
Note: You may have to additionally configure your router and Mac Preferences in order to access your localhost across your network. We do not provide support for this.
</div>

---

### Local ip with only localhost

If you only have a localhost, and no additional hosts, then accessing your host from a different Mac or mobile device can be done by entering the internal ip of your Mac. 

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLAN/localhost.png)

Type in the local ip of Mac with your MAMP PRO installed and running to access your localhost. This can be done from a mobile device or other Mac. 

<div class="alert" role="alert">
Note: You need to include the port Apache is running on. If you run Apache on the default port 80, then you do not need to enter a port number.
</div>

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLAN/host.png)

To find your local ip go to System Preferences > Network. Your local ip address is shown under "Status". 

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLAN/ip.png)

<div class="alert" role="alert">
Note: Your local ip address may change periodically, depending on your router settings. 
</div>

---

#### Multiple Hosts

When adding multiple hosts you need to comment out the following two lines in your Apache template file, in order to access your localhost, from other Macs and mobile devices. 

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLAN/template.png)

You can reach your Apache template file via the MAMP PRO menu, File > Edit Template > Apache > httpd.conf

---

#### From A Mobile Device

You can reach your localhost via a local ip using your mobile browser.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLAN/mobile.png)

---

### Accessing localhost using a Local Hostname

You can use a Mac's Local Hostname to access your localhost on another Mac on your LAN,  To find out the Local Hostname of this Mac, go to System Preferences > Sharing > Edit.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLAN/LocalHostName.png)

To access your localhost from a different Mac on your LAN. Input :8888 (assuming your are using Apache port 8888) as a suffix in your url bar.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLAN/LocalHostPage.png)

