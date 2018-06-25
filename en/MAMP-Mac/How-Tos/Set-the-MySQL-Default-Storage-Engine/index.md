---
title: MAMP (Mac) Documentation > How Tos > Set the MySQL Default Storage Engine
description: Set the MySQL Default Storage Engine
layout: default-2
product: MAMP Mac
language: en
---

## How Tos > Set the MySQL Default Storage Engine

The MySQL server of MAMP uses the Default Storage Engine MyISAM.
If you want to change this to a different storage engine such as InnoDB
you have to change the configuration file of the MySQL server.

1. Stop the MAMP Servers that are running.
2. Use a text editor to create a file named my.cnf and save it to the /Applications/MAMP/conf folder.
3. Add the following lines into the file:  
    `[mysqld]default-storage-engine = InnoDB`
4. Save the file and close your editor.
5. Start the MAMP servers.
