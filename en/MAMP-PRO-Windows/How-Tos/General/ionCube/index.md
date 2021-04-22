---
title: MAMP PRO (Windows) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Windows
language: en
lastedit: 2021-03-26
---

### Install ionCube

This example uses PHP 5.6.31. Please be aware if you are installing ionCube for a different PHP version you will need to use a different ionCube file versio and install to the corresponding PHP version directory.

1. Download the Windows VC11 (32 bits) tar.gz version of [ionCube](http://downloads3.ioncube.com/loader_downloads){:target="_blank"}. 
2. Unpack ioncube_loaders_win_vc11_x86.tar.gz. In your resulting "ioncube" directory there will be several files. Copy only the ioncube_loaders_win_5.6.dll file to "C:\MAMP\bin\php\php5.6.31\ext". The ioncube_loaders_win_5.6.dll is good for all PHP 5.6.x versions.
3. Add the following line to your PHP 5.6.31 template file. You can reach your template files in MAMP PRO through the menu bar, File > Edit Template > PHP > 5.6.31. 
4. Restart your servers in MAMP PRO.
5. To verify ionCube is loaded use your php.ini file. You should see the following in your php.ini file.
![MAMP](/en/MAMP-PRO-Mac/How-Tos/General/ionCubephpini.png)