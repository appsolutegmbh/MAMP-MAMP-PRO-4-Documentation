---
title: MAMP PRO (Mac) Documentation > How Tos > MySQL
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Connect To MySQL using Perl 

{% highlight php %}

use DBI;
 
my $user = 'root';
my $password = 'root';
my $db = 'inventory';

my $link = DBI->connect(
   "DBI:mysql:database=$db", 
   $user, 
   $password
);

{% endhighlight %}

or connecting via network:

{% highlight php %}

use DBI;
 
my $user = 'root';
my $password = 'root';
my $db = 'inventory';
my $host = 'localhost';
my $port = 8889;

my $link = DBI->connect(
   "DBI:mysql:database=$db;host=$host;port=$port", 
   $user, 
   $password
);

{% endhighlight %}
