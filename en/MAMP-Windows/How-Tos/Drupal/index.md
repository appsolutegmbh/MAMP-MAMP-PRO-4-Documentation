---
title: MAMP (Windows) Documentation > How Tos > Drupal
description: 
layout: default-2
product: MAMP Windows
language: en
---

## How to install Drupal

### Download Drupal and setup document root

Download Drupal [here](https://drupal.org){:target="_blank"} . After downloading, the resulting zip file should be in your `C:\Downloads` folder. Unzip this drupal.zip file. You should now see a `C:\Downloads\Drupal` folder. Move the contents of this folder  to `C:\Applications\MAMP\htdocs`.

### Create database

Click on Open Start Page, then on the phpMyAdmin link. Create a database in phpMyAdmin and call it "drupal".

![MAMP](/en/MAMP-Windows/How-Tos/Drupal/phpMyAdminDrupal.png)

### Run Drupal installation

Go to Open Start Page, click on "MyWebsite" on the top menu bar, you should now see the Drupal installation process begin.

![MAMP](/en/MAMP-Windows/How-Tos/Drupal/MyWebsiteLink.png)

The following fields are the default for the MAMP PRO MySQL installation, username: "root", password: "root", database host: "localhost" and port to 8889.

![MAMP](/en/MAMP-Windows/How-Tos/Drupal/drupalWizard1.png)

Finish the Drupal installation process. The "admin" user is the administration user for this Drupal site. You can use a different administrator user name other than "admin".

![MAMP](/en/MAMP-Windows/How-Tos/Drupal/drupalWizard2.png)
