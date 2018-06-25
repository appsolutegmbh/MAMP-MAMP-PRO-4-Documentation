---
title: MAMP PRO (Mac) Documentation > How Tos > General > Accessing localhost on a LAN using ports
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Accessing MAMP PRO hosts on A LAN using ports

You can access MAMP PRO hosts, other than localhost on a LAN using ports.

<div class="alert" role="alert">
Note: You may have to additionally configure your router and Mac Preferences in order to access your hosts across your network. We do not provide support for this.
</div>

---

You first need to set up your host that will be accessed from another mobile device or Mac on your LAN. This host must have the ip address and port set to a port other than the default Apache port you are using in MAMP PRO. In the following example, the port used for 'MySecondHost' is 8000. The Apache port used is 8888.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLANOtherHostsPorts/MySecondHost.png)

To access your localhost on another Mac on your LAN, you need to type in it's Local Hostname. To find out the Local Hostname of this Mac, go to System Preferences > Sharing > Edit .

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLANOtherHostsPorts/LocalHostName.png)

---

Now you can access your hosts from a different Mac on your LAN. Input :8888 as a suffix in your url bar to see the localhost. 

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLANOtherHostsPorts/LocalHostPage.png)

Type in :8000 in your url bar to see 'MySecondHost'.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/AccessingOnLANOtherHostsPorts/MySecondHostPage.png)





