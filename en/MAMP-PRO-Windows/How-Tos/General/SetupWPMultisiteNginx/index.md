---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Setup Multisite with a Wordpress host and Nginx using Subdomains

Setting up a Wordpress multisite is possible in MAMP PRO. Because Nginx does not use a .htaccess file, several additions to the location directive in Nginx will have to be made.

First set your Nginx port to port 80. Make a new host and set this host to Nginx. Manually install Wordpress or use the Extras feature in MAMP PRO. Enable "Multisite" in Wordpress by adding the following directly under WP_DEBUG to your wp-config.php file. Your wp-config.php file is in your document root folder.
 
 {% highlight php %}
  define('WP_ALLOW_MULTISITE', true);
 {% endhighlight %}
 
Go to you Nginx tab add the following to your "try files:" location parameter.

 {% highlight php %}
  $uri $uri/ /index.php?$args;
 {% endhighlight %}
 
Add the following to your location parameter.

{% highlight php %}
  location ~ ^/files/(.*)$ {
                try_files /wp-content/blogs.dir/$blogid/$uri /wp-includes/ms-files.php?file=$1 ;
                access_log off; log_not_found off;      expires max;
        }

    #WPMU x-sendfile to avoid php readfile()
 location ^~ /blogs.dir {
        internal;
        alias /var/www/example.com/htdocs/wp-content/blogs.dir;
        access_log off;     log_not_found off;      expires max;
    }
{% endhighlight %}

Add the following to your Nginx template file directly above the "server" directive.

{% highlight php %}
  map $http_host $blogid {
   default       -999;

   #Ref: http://wordpress.org/extend/plugins/nginx-helper/
   #include /var/www/wordpress/wp-content/plugins/nginx-helper/map.conf ;
	}
{% endhighlight %}
 
Restart your servers and navigate to the adminstration section of your Wordpress site. You can now add Multisite to your Wordpresss site. We have a video on how to do that here
 
 ![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/SetupWPwithNginx/permalinks.png)
 


