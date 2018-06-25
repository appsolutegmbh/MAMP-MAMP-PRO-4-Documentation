---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Redirect http traffic to https site using MAMP PRO interface

In order to redirect access from http to https, you must first setup both a [http and https host with the same host name](../SetUpHostHttpHttps).

1. Go to your Settings > Hosts > Apache tab in MAMP PRO.
2. Add the following lines to your Additional Parameters for <Virtual Host> directive:

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/httpsRedirectInMAMP.png)

{% highlight php %}

RewriteEngine On
RewriteCond %{HTTPS} off
RewriteRule (.*) https://%{SERVER_NAME}/$1 [R,L]

{% endhighlight %}

