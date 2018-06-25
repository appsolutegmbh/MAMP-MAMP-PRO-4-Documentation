---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Install a PHP extension using PECL

Use the following guideline to compile your own extensions. This example uses the mongodb extension and PHP 7.0.15. You can find more PHP extensions [here](https://pecl.php.net){:target="_blank"}.

1. Check the "Make this version available on the command line" check box on your Languages > PHP tab.
2. Restart your servers. A PECL alias now exists in your `~/.profile` file.
3. Open Terminal.app (/Applications/Utilities) and enter the following line into the terminal and hit enter:  
   `pecl install mongodb`
Your extension should now build and you should see the following result. 
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/buildResult.png) 
4. A mongodb.so extension should now be in your `/Applications/MAMP/bin/php/php7.0.15/lib/php/extension/no-debug-non-zts` folder.
5. Go to File > Edit Templates > PHP > PHP7.0.15 and add extension=mongodb.so.
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/addToTemplate.png)
6. Restart your servers and verify the extension has been loaded by checking phpInfo.
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/phpIniResult.png)




