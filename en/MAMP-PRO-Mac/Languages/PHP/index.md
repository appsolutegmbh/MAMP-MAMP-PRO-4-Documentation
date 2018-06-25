---
title: MAMP PRO (Mac) Documentation > Languages > PHP
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Languages > PHP

PHP is a popular web scripting programming language. MAMP PRO installs several versions of the PHP script interpreter.

![MAMP](/en/MAMP-PRO-Mac/Languages/PHP/php.png)

---

*  **Default version**  
   Select which PHP version will be the default version. To view the [php template file](../../Menu/File) press the ![MAMP](/en/MAMP-PRO-Mac/First-Steps/BlackArrow.png) button. Additional versions of php can be downloaded by pressing the ![MAMP](/en/MAMP-PRO-Mac/First-Steps/Plus.png) button.

   ![MAMP](/en/MAMP-PRO-Mac/Languages/PHP/phpUpdates.png)
   
   <div class="alert" role="alert">
      Note: To remove unneeded PHP versions simply stop your servers, quit MAMP PRO, and remove your /Applications/MAMP/bin/php/phpX.XX directory, where X.XX is the version of PHP you want removed. 
   </div>
   
   More information on removing PHP versions can be found [here](../../How-Tos/General/RemovePHPVersions).
   
---

<i class="fa fa-play-circle-o fa-lg" aria-hidden="true"></i> [Adding Additional PHP Versions](https://www.youtube.com/watch?v=5JZ3PSGj81E){:target="_blank"}

---

*  **Make this version available on the command line**  
   Check this option to make the current PHP version available on the command line. MAMP PRO uses aliases to provide this functionality. When this option is checked the following is added to your `~/.profile` file (PHP 7.1.1).
   
{% highlight php %}

alias php='/Applications/MAMP/bin/php/php7.1.1/bin/php -c "/Library/Application Support/appsolute/MAMP PRO/conf/php7.1.1.ini"'
alias pear='/Applications/MAMP/bin/php/php7.1.1/bin/pear'
alias pecl='/Applications/MAMP/bin/php/php7.1.1/bin/pecl'

{% endhighlight %} 


Confirm your php is enabled by typing "php -v" in your terminal.

![MAMP](/en/MAMP-PRO-Mac/Languages/PHP/terminalType.png)

![MAMP](/en/MAMP-PRO-Mac/Languages/PHP/terminalVersion.png)

<div class="alert" role="alert">
      Note: Your version of PHP on the command line is not configured by your PHP templates, or the MAMP PRO interface. 
</div>

More information on configuring your command line PHP can be found [here](../../Troubleshooting/General/General7).

---

*  **Mode**  
   Choose whether to use identical PHP versions for all hosts (module mode) or on a host by host basis (CGI mode).  

    *  **Identical PHP versions for all hosts (module mode)**  
       In module mode all hosts use the same PHP version.
    *  **Individual PHP version for every host (CGI mode)**  
       In CGI Mode the PHP settings will be identical for all hosts – except for the PHP version.
       Navigate to the Hosts section to change the PHP version for each individual host.
       More information on how to [change the PHP version for an individual host](../../Settings/Hosts/General/#setting_php_version) is covered in the Settings > Hosts > General section.  

---

*  **Cache module to speed up PHP execution**  
   PHP has several cache extensions that can help speed up execution in certain circumstances.
   This is set to "off" by default. Enabling a cache extension does not necessarily translate into greater execution speed.     A particular cache is not available for the current PHP version if it is not enabled.  

    *  **off**  
         No cache will be used.
   *  **APC**  
         The Alternative PHP Cache (APC) is a free and open opcode cache for PHP. You can learn more about APC [here](http://php.net/manual/en/book.apc.php){:target="_blank"} .
   *  **eAccelerator**  
         eAccelerator a free open-source PHP accelerator & optimizer. You can learn more about eaccelerator [here](http://eaccelerator.net){:target="_blank"}.
   *  **XCache**  
         XCache is a open-source opcode cacher. You can learn more about xCache [here](https://xcache.lighttpd.net){:target="_blank"}.
   *  **OPCache**  
         OPcache improves PHP performance by storing precompiled script bytecode in shared memory, thereby removing the need for PHP to load and parse scripts on each request. You can learn more about OPcache  [here](http://php.net/manual/en/book.opcache.php){:target="_blank"}.
   
   ![MAMP](/en/MAMP-PRO-Mac/Languages/PHP/cache.png) 
   
   Several caches provide a user interface to help analyze and profile your code. Press the ![MAMP](/en/MAMP-PRO-Mac/First-Steps/BlackArrow.png) button to the right of the cache name to view this interface. An interface is not available if the Arrow button is not enabled.

---

*  **Extensions**  

    *  **Xdebug (Debugger)**  
       Activate Xdebug to allow PHP to create debugging information during script execution.
       By default, Xdebug uses localhost and port 9000 in the PHP.ini file. More information on using Xdebug with the MacGDBp Debugger can be founder [here](../../How-Tos/General/UseXdebug). 

    *  **Imagick / ImageMagick**  
       Activate Imagick / ImageMagick.
       
    *  **Tidy**  
       Activate Tidy.
       
    *  **Oauth**  
       Activate Oauth.
    
    *  **Open MacGDBp**  
       With Xdebug activated you can open the MacGDBp debugger to enable PHP debugging.
       By default, MacGDBp expects debugging information on port 9000 of localhost. More information on using Xdebug with the MacGDBp Debugger can be founder [here](../../How-Tos/General/UseXdebug). 

---

*  **What to log**  
   Determine which error types should be reported.  

    *  **Display startup errors**  
       Log PHP errors that occur when Apache loads the PHP module.  

    *  **All errors and warnings**  
       All errors will be reported.  

    *  **Errors**  
       Script errors that make the further execution of the current PHP script impossible.  

    *  **Warnings**  
       General errors in the PHP environment.  

    *  **Notices**  
       Possible problems, that do not concern PHP, but which could be a notice of an error in a script.  

    *  **Other**  
       Report further error types through constants. Please turn to the PHP documentation for further information.

---

*  **Log Errors**  
   Determine if errors should be recorded in a log file and/or displayed in a web browser window.

---

More information on how to [connect to MySQL using PHP (PHP <= 5.5.x)](../../How-Tos/MySQL/#php_connect_mysql) can be found in our How To section.


More information on how to [connect to MySQL using PHP (PHP >= 5.6.x) ](../../How-Tos/MySQL/#php_connect_mysqli) can be found in our How To section.

