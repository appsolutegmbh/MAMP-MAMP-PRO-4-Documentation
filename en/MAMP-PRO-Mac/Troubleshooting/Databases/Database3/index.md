---
title: MAMP PRO (Mac) Documentation > MySQL and Database Troubleshooting
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### My MySQL Server is slow

You can diagnose why your MySQL is slow by adding the following to your my.cnf template file below [mysqld]. 

{% highlight php %} 
slow-query-log = 1
slow-query-log-file = /applications/mamp/logs/mysql-slow.log
long_query_time = 1
log-queries-not-using-indexes {% endhighlight %}

Restart your MySQL server. Access your database. You should now see a log file named mysql-slow.log in your  `/Applications/MAMP/logs` directory.





