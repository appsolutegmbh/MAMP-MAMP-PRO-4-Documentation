---
title: MAMP PRO (Mac) Documentation > Apache Troubleshooting
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Apache Troubleshooting

### My Apache Server will not start?

#### Another mysql service running

The most common problem with Apache Server not starting is another mysql service running on the same port. To check this

1. Quit MAMP PRO.
2. Open the Activity Monitor located in your /Applications/Utilities folder.
3. Type "httpd" into the search field on the top right.
4. Quit every process you find after your search.
5. Restart MAMP PRO.
6. If Apache still refuses to start check the log file for error messages.

---

#### Skype is running

Skype listens on port 80 and 443. You cannot run your MAMP PRO instance of Apache on port 80 while using Skype.


