---
title: MAMP PRO (Windows) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### Increase the PHP memory limit

1. Start MAMP PRO
2. Stop the server if it's running 
3. Choose Menu > File > Edit Template > PHP 5.x.x php.ini / PHP 5.x.x php.ini
4. The PHP ini file will be opened.
5. If a dialogue box pops up, read it and confirm with OK
6. Search (<kbd>Command</kbd> + <kbd>F</kbd>) for `memory_limit`
7. You should get the following line:  
   `memory_limit = 32M ; Maximum amount of memory a script may consume (8M)' 
8. Now you can change the default value of `32M`. For instance into `64M` or even more (like `128M`)
9. Save (<kbd>Command</kbd> + <kbd>S</kbd>) your changes.
10. Close (<kbd>Command</kbd> - <kbd>W</kbd>) the file.
11. Start the Server.
