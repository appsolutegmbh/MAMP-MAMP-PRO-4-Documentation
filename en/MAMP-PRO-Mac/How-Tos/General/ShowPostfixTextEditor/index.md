---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Show the Postfix log file With a text editor 

<div class="alert" role="alert">
Note: If you want to open the Postfix log file with a text editor, you have to make the file visible.
</div>

1. Open the Terminal.app (Applications/Utilities)
2. Enter the following and hit enter:  
   `defaults write com.apple.finder AppleShowAllFiles -boolean true`
3. Restart the Finder by enter the following and hit enter:  
   `killall Finder`
4. Open the file /private/var/log/mail.log with your editor.

