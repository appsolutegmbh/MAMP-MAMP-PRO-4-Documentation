---
title: MAMP PRO (Mac) Documentation > How Tos > MySQL
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Set the MySQL Default Storage Engine

The MySQL server of MAMP PRO uses the Default Storage Engine MyISAM. If you want to change this, you have to change the configuration file of the MySQL server. With this tutorial we want to show you how to manage this. As Default Storage Engine we are using InnoDB.

1. Start MAMP PRO.
2. Stop the MAMP PRO server if it is running. 
3. Select File > Edit Template > MySQL my.cnf 
4. An editor window appears.
5. If a warning message appears confirm with OK.
6. Find the section `[mysqld]`
7. Beneath the last line of this section add this line:  
   `default-storage-engine = InnoDB`
8. The section `[mysqld]` now looks like this:  
   IMAGE
9. Save (<kbd>Apple</kbd> + <kbd>S</kbd>) all changes made on "my.cnf"
10. Close the editor window (<kbd>Apple</kbd> + <kbd>W</kbd>)
11. Start the MAMP PRO servers.

---


