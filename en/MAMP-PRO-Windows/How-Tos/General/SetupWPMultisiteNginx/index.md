---
title: MAMP PRO (Windows) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Setup Multisite with a WordPress host and Nginx using Subdomains

Setting up a WordPress multisite is possible in MAMP PRO. Because Nginx does not use a .htaccess file, several additions to the location directive in Nginx will have to be made.

First set your Nginx port to port 80. Make a new host and set this host to Nginx. Manually install WordPress or use the Extras feature in MAMP PRO. Enable "Multisite" in WordPress by adding the following directly under WP_DEBUG to your wp-config.php file. Your wp-config.php file is in your document root folder.
 
```php
define('WP_ALLOW_MULTISITE', true);
```
 
Go to you Nginx tab add the following to your "try files:" location parameter.

```
$uri $uri/ /index.php?$args;
```
 
Add the following to your location parameter.

```
location ~ ^/files/(.*)$ {
  try_files /wp-content/blogs.dir/$blogid/$uri /wp-includes/ms-files.php?file=$1 ;
  access_log off;
  log_not_found off;
  expires max;
}

#WPMU x-sendfile to avoid PHP readfile()
location ^~ /blogs.dir {
  internal;
  alias /var/www/example.com/htdocs/wp-content/blogs.dir;
  access_log off;
  log_not_found off;
  expires max;
}
```

Add the following to your Nginx template file directly above the "server" directive.

```
map $http_host $blogid {
  default -999;

  #Ref: http://wordpress.org/extend/plugins/nginx-helper/
  #include /var/www/wordpress/wp-content/plugins/nginx-helper/map.conf ;
}
```
 
Restart your servers and navigate to the adminstration section of your WordPress site. You can now add Multisite to your WordPress site. We have a video on how to do that here
 
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/SetupWPwithNginx/permalinks.png)
 


