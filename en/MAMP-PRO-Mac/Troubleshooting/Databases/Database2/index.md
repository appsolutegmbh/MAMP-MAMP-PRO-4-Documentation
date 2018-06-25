---
title: MAMP PRO (Mac) Documentation > MySQL and Database Troubleshooting
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### My MySQL Server will not start and I am getting the following error in my mysql error log located in /Applications/MAMP/logs .

This may occur when your Mac goes to sleep.

10:12:32 1753 [Note] InnoDB: The log sequence numbers 609248312 and 609248312 in ibdata files do not match the log sequence number 609248322 in the ib_logfiles!


1. Quit MAMP PRO.
2. Go to your `/Library/application support/appsolute/MAMP PRO/db/mysql56` directory.
3. Rename both ib_logfile0 and ib_logfile1.
4. Restart MAMP PRO.
5. Both ib_logfile0 and ib_logfile1 should be rebuilt.

