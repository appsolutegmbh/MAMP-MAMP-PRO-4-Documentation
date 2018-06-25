---
title: MAMP PRO (Mac) Documentation > General Troubleshooting
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Command line PHP extensions are not showing up when I run PHP from the command line.

Your command line PHP uses a php.ini file located within the `/Applications/MAMP` directory.

When using command line PHP, to include extensions that you wish to use, add them to the corresponding version number. For instance, PHP 7.1.1 would use the following php.ini file located in`/Applications/MAMP/bin/php/php7.1.1/conf`.

To see where your command line php.ini file is located, type the following in the terminal. 

![MAMP](/en/MAMP-PRO-Mac/Troubleshooting/General/General7/phpVersion.png)

![MAMP](/en/MAMP-PRO-Mac/Troubleshooting/General/General7/phpVersionResult.png)






