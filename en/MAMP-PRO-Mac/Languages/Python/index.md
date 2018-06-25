---
title: MAMP PRO (Mac) Documentation > Languages > Python
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Languages > Python

Python is a widely used high-level, general-purpose, interpreted, dynamic programming language. MAMP PRO installs Python in your  `/Applications/MAMP/Library/bin/python` directory. MAMP PRO will not make any changes to the Python build that is pre installed on your Mac. The Apple-provided build of Python is installed in `/usr/bin/python`.

![MAMP](/en/MAMP-PRO-Mac/Languages/Python/Python.png)

---

*  **Make Python available on the command line**  
      Check this option to make the current Python version available on the command line. MAMP PRO uses an alias to provide this functionality. When this option is checked the following is added to your `~/.profile` file.
   
   
{% highlight php %}

alias python='/Applications/MAMP/Library/bin/python'

{% endhighlight %} 
 

---

More information on how to [connect to MySQL using Python](../../How-Tos/MySQL/ConnectMySQLPython/) can be found in our How To     section.
