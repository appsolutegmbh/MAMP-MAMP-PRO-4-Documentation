---
title: MAMP (Mac) Documentation > FAQ
description: 
layout: default-2
product: MAMP Mac
language: en
---

## FAQ

### How do I access my preferences?

You can access your preferences through the menu bar. Go to MAMP > Preferences. 

---

#### Is MAMP compatible with Mac OS X 10.11 (El Capitan), Mac OS 10.12 (Sierra), and Mac OS 10.13 (High Sierra)?

Yes, MAMP is compatible with all of these operating systems. 

---

### Where can I download MAMP?

Get the latest version of MAMP from our website [https://www.mamp.info/en/downloads/](https://www.mamp.info/en/downloads/){:target="_blank"}.

---

### Where can I find the log files?

All log files are stored in: `/Applications/MAMP/logs/`.

---

### Which Apache modules are included?

Apache modules are located in the `/Applications/MAMP/Library/modules` folder.

---

### Which PHP modules are included?

To find out which PHP modules are included, use the following procedure:

Start the servers and direct your web browser to http://localhost:8888/MAMP/.
Click on the phpInfo tab at the top of page.

---

<a name="cloud"> </a>

### What does the following warning message mean when I load cloud data?

![MAMP](/en/MAMP-Mac/FAQ/DatabaseWarning.png)

This is only a warning message indicating that the MySQL user associated with the database getting loaded from the cloud already exists on your local machine.

---

### What does the following error message mean when I save cloud data?

![MAMP](/en/MAMP-Mac/FAQ/DatabaseError.png)

The following error message means the database you are attempting to save to the cloud does not have a MySQL user associated with it. You must first associate a user with this database in order to save it to the cloud. 

An associated user can be added in phpMyAdmin.


1) Create a database named “wordpress”, for example:

![MAMP](/en/MAMP-Mac/FAQ/step1.png)

2) After Adding the database, go to the User Accounts tab and click "Add User:".

![MAMP](/en/MAMP-Mac/FAQ/step2.png)

3) Add a new User and add all global privileges; click "Go":

![MAMP](/en/MAMP-Mac/FAQ/step3.png)

4) With the userX created, click "Edit Privileges".

![MAMP](/en/MAMP-Mac/FAQ/step4.png)

5) Add all privileges to userX and click "Go".

![MAMP](/en/MAMP-Mac/FAQ/step5.png)

6) Inside the userX privileges, click "Database".

![MAMP](/en/MAMP-Mac/FAQ/step6.png)

7) Select the database, in our case, “wordpress”, and click "Go".

![MAMP](/en/MAMP-Mac/FAQ/step7.png)

8) Add all the privileges for userX uses the database “wordpress”, and click "Go".

![MAMP](/en/MAMP-Mac/FAQ/step8.png)
 
9) Now, for the database “wordpress”, our userX now has all privileges.

![MAMP](/en/MAMP-Mac/FAQ/step9.png)

