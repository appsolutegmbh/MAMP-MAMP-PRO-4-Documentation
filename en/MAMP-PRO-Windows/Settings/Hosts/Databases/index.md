---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > Extras
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Settings > Hosts > Databases

The Database tab indicates which databases are associated with each host. You can associate individual databases or tables with a host. Disabled checkmarks flag databases and tables that are mapped to a host via an Extra.

![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/Databases/Databases.PNG)

---

### New Database

Press the '+' button to add a new database. It is only possible to add databases, and not individual tables.

![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/Databases/newDatabases.PNG)


   *  **Name of new database**
   
      This is your MySQL database name.
   
   *  **Grant access to user**
   
      When you do grant access, you have the choice of using an existing user, or your can create a new user. If you choose to create a new MySQL user, a password for this new MySQL user is required. This must be filled in below in the "Using password" text field. If an existing MySQL user is chosen, the "using password" field is disabled, and the existing password of this MySQL user will automatically be used. If this box is not checked, the new database will be created by and rights given to the MySQL "root" user.
   
   *  **Using password**
   
      The password for your MySQL user. When a new MySQL user is created a password is needed to continue. This field is disabled if an existing MySQL database user is creating the database.
 


