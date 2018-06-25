---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Use Nginx as reverse proxy for Apache while redirecting to a host other than localhost

When you check the "Use Nginx as a Reverse Proxy for Apache" check box in Settings > Hosts > Nginx, by default your Nginx php scripts will be redirected to localhost. You can direct your php scripts to a host other than localhost by making two small changes in your Nginx template file and MAMP PRO interface.

1. Change the port number of the Apache host you want PHP scripts to be redirected to.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/changePort.png)

2. In your Nginx template change the port number to reflect the port number change in your Apache host.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/templatePort.png)





