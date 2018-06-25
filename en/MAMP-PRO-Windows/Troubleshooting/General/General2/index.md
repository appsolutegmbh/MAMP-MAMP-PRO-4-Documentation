---
title: MAMP PRO (Windows) Documentation > General Troubleshooting
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

### My Apache Server will not start?

The most common problem with Apache Server not starting is another mysql service running on the same port. To check this

1. Quit MAMP PRO.
2. Open the Windows Task Manager.
3. Go to the Processes tab.
4. Type "httpd" into the search field on the top right.
5. Quit every process you find after your search.
5. Restart MAMP PRO.

If Apache still refuses to start check the log file for error messages.
