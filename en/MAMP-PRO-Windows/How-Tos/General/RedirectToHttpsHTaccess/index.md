---
title: MAMP PRO (Windows) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### Redirecting http traffic to https site using .htaccess file

1. Create a .htaccess file using the MAMP PRO Editor and save this file in your document root.
2. Add the following lines to your .htaccess file.

```
<ifmodule mod_rewrite.c="">  
RewriteEngine On   
RewriteCond %{HTTPS} off    
RewriteRule (.*) https://%{HTTP_HOST}%{REQUEST_URI} [R=301,L]    
</ifmodule>    
```