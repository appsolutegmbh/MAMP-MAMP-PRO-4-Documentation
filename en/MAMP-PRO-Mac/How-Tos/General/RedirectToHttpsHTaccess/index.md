---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Redirecting http traffic to https site using .htaccess file

In order to redirect access from http to https, you must first setup both a [http and https host with the same host name](../SetUpHostHttpHttps).


1. Create a .htaccess file using the MAMP PRO Editor and save this file in your document root.
2. Add the following lines to your .htaccess file.

![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/httpsRedirect.png)

{% highlight php %}

<ifmodule mod_rewrite.c="">  
RewriteEngine On   
RewriteCond %{HTTPS} off    
RewriteRule (.*) https://%{HTTP_HOST}%{REQUEST_URI} [R=301,L]    
</ifmodule>    

{% endhighlight %}





