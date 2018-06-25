---
title: MAMP PRO (Windows) Documentation > General Troubleshooting
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### My PHP scripts are timing out


If your PHP scripts are timing out you may have to adjust one of the following PHP directives in your PHP template file.

{% highlight php %} 
max_execution_time = 600     ; Maximum execution time of each script, in seconds
max_input_time = 600    ; Maximum amount of time each script may spend parsing request data
{% endhighlight %}
WHen using CGI PHP, you must add this additional variable to your PHP template file to prevent PHP from timing out after 30 seconds.
{% highlight php %} 
default_socket_timeout = 600
{% endhighlight %}
