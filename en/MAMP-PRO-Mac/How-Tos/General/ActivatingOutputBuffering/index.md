---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Activating Output Buffering

1. Start MAMP PRO
2. Select File -> Edit Template -> PHP 5.x.x php.ini / PHP 5.x.x php.ini 
3. Search this line  
   `output_buffering = Off`
4. Change `Off` to `On` or to a maximum number of bytes instead (for example `4096`)
5. Save the file
6. Start servers
