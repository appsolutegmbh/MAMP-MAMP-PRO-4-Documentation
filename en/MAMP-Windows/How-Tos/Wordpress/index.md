---
title: MAMP (Windows) Documentation > How Tos > WordPress
description: 
layout: default-2
product: MAMP Windows
language: en
lastedit: 2021-03-26
---

## How To install WordPress

### Download WordPress and setup document root

First Download WordPress [here](https://wordpress.org){:target="_blank"}. After downloading, the resulting zip file should be in your "C:\Downloads" folder. Unzip this WordPress.zip file. You should now see a "C:\Downloads\WordPress" folder. Move the contents of this folder to "C:\MAMP\htdocs".

### Create database

Click on Open Start Page, then on the phpMyAdmin link. Create a database in phpMyAdmin and call it "wordpress".

![MAMP](/en/MAMP-Windows/How-Tos/WordPress/phpMyAdminAddWordPress.png)

### Run WordPress installation

Go to Open Start Page, click on "MyWebsite" on the top menu bar, you should now see the WordPress installation process begin.

![MAMP](/en/MAMP-Windows/How-Tos/WordPress/MyWebsiteLink.png)

The following fields are the default for the MAMP PRO MySQL installation, user name: "root", password: "root", database host: "localhost:8889" (Use only "localhost" if your MySQL port is 3306)

![MAMP](/en/MAMP-Windows/How-Tos/WordPress/WordPressWizard.png)

Finish the WordPress installation process. The "admin" is your WordPress administrator. You can use a different user name for the administrator.

![MAMP](/en/MAMP-Windows/How-Tos/WordPress/WordPressWizard2.png)