---
title: MAMP PRO (Windows) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### Redirect http traffic to https site using MAMP PRO interface

1. Go to your Settings > Hosts > Apache tab in MAMP PRO.
2. Add the following lines to your Additional Parameters for <Virtual Host> directive:

![MAMP](/en/MAMP-PRO-Windows/How-Tos/General/RedirectToHttpsMAMPPRO/RedirectToHttpsMAMP.png)

{% highlight php %}

RewriteEngine On
RewriteCond %{HTTPS} off
RewriteRule (.*) https://%{SERVER_NAME}/$1 [R,L]

{% endhighlight %}

