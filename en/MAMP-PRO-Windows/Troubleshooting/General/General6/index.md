---
title: MAMP PRO (Windows) Documentation > General Troubleshooting
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### I cannot see my localhost using the Edge browser

Microsoft Edge allows localhost access by default but treats "localhost" as an Internet site, so Intranet features like integrated authentication are disabled. You must run the following command in your terminal to view localhost.

`CheckNetIsolation LoopbackExempt -a -n="Microsoft.MicrosoftEdge_8wekyb3d8bbwe"`

More information on localhost and Microsoft Edge can be found here.

[https://developer.microsoft.com/en-us/microsoft-edge/platform/faq/#how-can-i-debug-localhost](https://developer.microsoft.com/en-us/microsoft-edge/platform/faq/#how-can-i-debug-localhost){:target="_blank"}
