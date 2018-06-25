---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Install Composer for a Individual Host

You can setup a host to use Composer in a few steps. Information on downloading Composer can be found [here](https://getcomposer.org/doc/00-intro.md){:target="_blank"}. Scroll down and click on  "download this file" for OS X. This should download an "Installer" file to your downloads folder. 

Next create a host. In a new terminal navigate to the document root of   your new host. Move the Install file which you downloaded from the Composer website to your document root. Run the following commands in your terminal found in the Composer documentation as explained [here](https://getcomposer.org/download/){:target="_blank"}.
 
 {% highlight php %}
  php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
    php -r "if (hash_file('SHA384', 'composer-setup.php') === '669656bab3166a7aff8a7506b8cb2d1c292f042046c5a994c43155c0be6190fa0355160742ab2e1c88d40d5be660b410') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
  php composer-setup.php
  php -r "unlink('composer-setup.php');"
 {% endhighlight %}
 
 You can find packages [here](https://packagist.org){:target="_blank"}.
  
 To install the psr/log, a common interface for logging libraries, type the following in your terminal and press return.
    
 {% highlight php %}
   php composer.phar require psr/log
 {% endhighlight %}
    
 Your document root should now look like the this.
    
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/SetupComposer/documentRoot.png)
    
---

