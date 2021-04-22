---
title: MAMP PRO (Windows) Documentation > How Tos > MySQL
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Connect to MySQL from PHP (PHP >= 5.6.x)

```php
$user = 'root';
$password = 'root';
$db = 'inventory';
$host = 'localhost';
$port = 8889;

$link = mysqli_init();
$success = mysqli_real_connect(
   $link, 
   $host, 
   $user, 
   $password, 
   $db,
   $port
);
```