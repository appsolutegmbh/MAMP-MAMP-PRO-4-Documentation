---
title: MAMP PRO (Windows) Documentation > How Tos > MySQL
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### Connect to MySQL from PHP (PHP <= 5.5.x)

```php
$user = 'root';
$password = 'root';
$db = 'inventory';
$host = 'localhost';
$port = 8889;

$link = mysql_connect(
   "$host:$port", 
   $user, 
   $password
);
$db_selected = mysql_select_db(
   $db, 
   $link
);
```