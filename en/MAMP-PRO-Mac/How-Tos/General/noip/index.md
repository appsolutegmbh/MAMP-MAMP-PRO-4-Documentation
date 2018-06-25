---
title: MAMP PRO (Mac) Documentation > How Tos > General > Dynamic DNS with noip.com
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Dynamic DNS with noip.com

You can set up dynamic dns with a free or paid account using noip.com. Your site will be visible to the internet when you set up dynamic dns correctly. 

<div class="alert" role="alert">
Note: We cannot provide support for setting up your dynamic dns with MAMP PRO.
</div>

In MAMP PRO, the host must (as an example we take 'testhostforclients.ddns.net') that will later be accessible from the Internet, be functioning properly. Check this by clicking in the host configuration on the right arrow next to the field "Name" on the Hosts tab. In the web browser, the host must appear.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/noip/hostsMAMPPRO.png)

Create an account on [www.noip.com](https://noip.com){:target="_blank"}. After you have successfully created an acount you can create a hostname. This host name must be identical to the one you created in MAMP PRO. In this example the host name is 'testhostforclients.ddns.net'.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/noip/hostName.png)

Set up port forwarding. If your MAMP PRO is installed on a Mac, connected to the Internet via a router, then a so-called port forwarding [http://en.wikipedia.org/wiki/Port_forwarding](http://en.wikipedia.org/wiki/Port_forwarding){:target="_blank"} must be set on this router. Other terms may be used for this such as "port sharing". Unfortunately, there is no universal protocol or method to set port forwarding. Terminology and methods differ from router to router. The following sets the forwarded port to 8888 on a speedport router.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/noip/portForwarding.png)

Start your servers in MAMP PRO, including your DNS service with the correct username and password provided.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/noip/dynDNS.png)

You should now be able to view your website from the internet. To confirm that your site is working properly, turn off Wifi on your mobile device, and then try accessing your site using your mobile data.



