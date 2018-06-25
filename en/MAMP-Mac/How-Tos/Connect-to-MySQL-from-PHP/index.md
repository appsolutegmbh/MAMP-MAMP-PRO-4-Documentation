---
title: MAMP (Mac) Documentation > How Tos > Connect to MySQL from PHP
description: Connect to MySQL from PHP
layout: default-2
product: MAMP Mac
language: en
---

## How Tos > Connect to MySQL from PHP

The following example shows how to connect to a MySQL database using the `mysqli()` library:

{% highlight php %}
<?php
  DEFINE('DB_USERNAME', 'root');
  DEFINE('DB_PASSWORD', 'root');
  DEFINE('DB_HOST', 'localhost');
  DEFINE('DB_DATABASE', 'performance_schema');

  $mysqli = new mysqli(DB_HOST, DB_USERNAME, DB_PASSWORD, DB_DATABASE);

  if (mysqli_connect_error()) {
    die('Connect Error ('.mysqli_connect_errno().') '.mysqli_connect_error());
  }

  echo 'Connected successfully.';

  $mysqli->close();
?>
{% endhighlight %}
