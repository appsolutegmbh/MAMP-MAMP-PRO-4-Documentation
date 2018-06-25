---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Create a host using the command line

You can create a host using the command by using the following steps

1. Quit MAMP PRO.
2. Open Terminal.app ( /Applications/Utilities ).
3. Enter the following line into the terminal and hit enter:  
   `/Applications/MAMP\ PRO/MAMP\ PRO.app/Contents/MacOS/MAMP\ PRO cmd createHost testHost /Applications/MAMP/htdocs2`
4. Enter the following line into the terminal and hit enter:
`/Applications/MAMP\ PRO/MAMP\ PRO.app/Contents/MacOS/MAMP\ PRO cmd createHost testHost /Applications/MAMP/htdocs2 testDB`
5. Enter the following command and hit enter: `/Applications/MAMP\ PRO/MAMP\ PRO.app/Contents/MacOS/MAMP\ PRO cmd stopServers`

This will create a host with the name ‘TestHost’, with a document root of ‘/Applications/MAMP/htdocs2’, and a database named ‘testDB’. MAMP PRO will briefly open both when the servers are started, stopped, as well as when the host is created. MAMP PRO will then quit again each time. When you re open MAMP PRO you will see your new host and database.
   





