---
title: MAMP PRO (Mac) Documentation > General Troubleshooting
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### My xip.io link does not work on other devices on my LAN?

To verify your xip.io is working cut and paste your xip.io address from MAMP PRO and type [nslookup xip.io host name ] on the command line

nslookup myhostName.xip.io

Your ip address should be returned. This means your xip.io is working properly.

You may also be having problems with your router settings. Make sure they are set properly to allow xip.io to function properly. The following are instructions for some router settings in Germany, your router may have similar settings that have to be changed.

---

AVM's FritzBox has a security feature that prevents DNS Servers to resolve anything in the FritzBox local IP range (Default 192.168.178.0/24)

try

dig 192.168.178.102.xip.io

and

dig 192.168.178.102.xip.io @8.8.8.8

You will see that it's the problem of the DNS server of the FritzBox as Google's DNS server (8.8.8.8) resolves the domain name just fine.

To use xip.io behind a FritzBox you have three options:

Configure your local computer to use the Google DNS (8.8.8.8). That's easy but then you cannot use the "fritz.box" domain name anymore.

Setup a local DNS resolver/forarder on a (linux) router in your local LAN and use this DNS server.

Install freetz (http://freetz.org/) and dnsmasq on your FritzBox. Add "xip.io" to "Heimnetz -> Netzwerk -> Netzwerkeinstellungen -> DNS-Rebind-Schutz" and you can use the build-in DNS server of the FritzBox and xip.io together.


