---
title: MAMP PRO (Mac) Documentation > How Tos > MySQL
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### How to transfer database data from MAMP to MAMP PRO

1. Stop your servers and close any instances of MAMP and MAMP PRO.
2. Open your Mac Finder and navigate to `/Library/application data/appsolute/MAMP PRO`.
3. Rename your `/db` folder to `/db_bak`.
4. Open MAMP PRO and launch your servers.

When MAMP PRO launched it's servers it (re) copied database data from the MAMP location to the MAMP PRO location because it did not detect a `/Library/application data/appsolute/MAMP PRO/db` folder. You should now be looking at your current database data.
