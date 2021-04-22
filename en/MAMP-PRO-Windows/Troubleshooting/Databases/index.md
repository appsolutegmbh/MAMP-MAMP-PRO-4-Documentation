---
title: MAMP PRO (Windows) Documentation > MySQL and Database Troubleshooting
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## MySQL and Database Troubleshooting

### My MySQL Server will not start?

#### Additional MySQL Process is running

The most common problem with MySQL Server not starting is another mysql service running on the same port. To check this 

1. Quit MAMP PRO.
2. Open the Task Manager.
3. Go to the processes tab.
3. Type "mysqld" into the search field on the top right.
4. Quit every process you find after your search.
5. Restart MAMP PRO.

If MySQL still refuses to start check the log file for error messages.

