---
title: MAMP PRO (Mac) Documentation > MySQL and Database Troubleshooting
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### My MySQL Server will not start?

The most common problem with MySQL Server not starting is another mysql service running on the same port. I may also be a mysql process started by MAMP PRO previously did not shut down properly when you quit MAMP PRO. To check this do the following. 

1. Quit MAMP PRO.
2. Open the Activity Monitor located in your /Applications/Utilities folder.
3. Type "mysqld" into the search field on the top right.
4. Quit every process you find after your search.
5. Restart MAMP PRO.
6. If MySQL still refuses to start check the log file for error messages.

