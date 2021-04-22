---
title: MAMP PRO (Windows) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### Change permalink settings with WordPress host and Nginx

Changing the permalink settings in WordPress when using Nginx will result in a 404 error when viewing your site. Add the following line to your "try files:" text box in Settings > Hosts > Nginx to fix this issue. 

```
$uri $uri/ /index.php?$args;
```
 
Restart your servers, close and reopen your browser. You will now see your individual posts instead of a 404 error when navigating through your WordPress site.
 
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/SetupWPwithNginx/permalinks.png)
 
More information about using WordPress with Nginx can be found [here](https://www.nginx.com/resources/wiki/start/topics/recipes/wordpress/){:target="_blank"}.