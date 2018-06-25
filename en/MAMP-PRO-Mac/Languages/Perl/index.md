---
title: MAMP PRO (Mac) Documentation > Languages > Perl
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Languages > Perl

Perl is a high-level, general-purpose, interpreted, dynamic programming language. A version 5 of Perl is included with MAMP PRO.

![MAMP](/en/MAMP-PRO-Mac/Languages/Perl/Perl.png)

*  **Make Perl directly available on the command line**  
   Check this option to make the current Perl version available on the command line. MAMP PRO uses aliases to provide this functionality. When this option is checked the following is added to your `~/.profile` file.
   
   
{% highlight php %}

alias perl='/Applications/MAMP/Library/bin/perl'
alias cpan='/Applications/MAMP/Library/bin/cpan'

{% endhighlight %} 
   
---

More information on how to [connect to MySQL using Perl](../../How-Tos/MySQL/#perl_connect) can be found in our How To section.
