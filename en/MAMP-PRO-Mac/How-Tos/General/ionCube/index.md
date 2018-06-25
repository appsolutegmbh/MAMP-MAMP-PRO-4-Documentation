---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Install ionCube

This example uses PHP 7.0.13. Please be aware if you are installing ionCube for a different PHP version you will need to use a different ionCube file version (dar_5.6 instead of dar_7.0) and install to the corresponding PHP version directory ( phpXXX instead of php7.0.13 ).

1. Download the OS X (64 bits) tar.gz version of [ionCube](http://downloads3.ioncube.com/loader_downloads/ioncube_loaders_dar_x86-64.tar.gz){:target="_blank"}. 
2. Unpack ioncube_loaders_darx86-64.tar.gz . In your resulting `ioncube` directory there will be several files. Copy only the ioncube_loader_dar_7.0.so file to `/Applications/MAMP/bin/php/php7.0.13/lib/php/extensions/no-debug-non-zts-20151012`. The ioncube_loader_dar_7.0.so is good for all PHP 7.0.x versions.
3. Add the following line to your php 7.013 template file. You can reach your template files in MAMP PRO through the menu bar, File > Edit Template > PHP > 7.0.13 . Be sure this line is above all other Zend directives.
zend_extension = /Applications/MAMP/bin/php/php7.0.13/lib/php/extensions/no-debug-non-zts-20151012/ioncube_loader_dar_7.0.so
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/phpTemplate.png)
4. Restart your servers in MAMP PRO.
5. To verify ionCube is loaded use your php.ini file. You should see the following in your php.ini file.
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/ionCubephpini.png)






