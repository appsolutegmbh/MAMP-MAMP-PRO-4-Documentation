---
title: MAMP PRO (Mac) Dokumentation
description: 
layout: default-2
product: MAMP PRO Mac
language: de
---

## Ablage

Einstellungen, die Sie in MAMP PRO vornehmen, werden beim Speichern in Konfigurationsdateien für die Server geschrieben. Dazu verwendet MAMP PRO Vorlagen, in denen auch weitere Konfigurationsoptionen fest enthalten sind. Sie können diese Vorlagen unter dem Menüpunkt Ablage > Vorlagen editieren und verändern. Dadurch können Sie auch auf Optionen zugreifen, die in der MAMP PRO Oberfläche nicht verfügbar sind.

<div class="alert" role="alert">
Hinweis: Fehler in den Vorlagen der Konfigurationsdateien können dazu führen, dass Server nicht mehr starten. Dies kann bedeuten, dass Sie MAMP PRO zurücksetzen müssen und alle Einstellungen verlieren. Sie sollten diese Vorlagen daher nur bearbeiten, wenn Sie mit der exakten Syntax und Bedeutung der Optionen vertraut sind!
</div> 

*Apache (httpd.conf and httpd-ssl.conf)*
     
Open and edit your httd.conf template file here. Changes made to your template file will be reflected your         real      httpd.conf file. The httpd.conf file created from the template file and is located in `/Library/appsolute/MAMP              PRO/conf`. You can check this file to verify changes you are making in your template file are properly reflected.
<div class="alert" role="alert">
Changes are reflected in your real httpd.conf file after your servers are restarted. This applies to all                    configuration files including nginx.conf, php.ini, my.cnf and main.cnf.
</div>
     
*Nginx (nginx.conf)*

Open and edit your nginx.conf template file here. Changes made to your template file will be reflected your                 real nginx.conf file. The nginx.conf file created from the template file and is located in `/Library/appsolute/MAMP         PRO/conf`.
     
*PHP (php.ini)*
     
Open and edit your php.ini template file here. There are likely several versions of php available, each of them with        their own template file. Changes made to your template file will be reflected your real php.ini file. The php.ini file      created from the template file and is located in `/Library/appsolute/MAMP PRO/conf`.
     
![MAMP](PHPini.png)
     
*MySQL(my.cnf)*
     
Open and edit your my.cnf template file here. There are likely several versions of MySQL available, each of them with       their own template file. Changes made to your template file will be reflected your real my.cnf file. The my.cnf file        created from the template file and is located in `/Library/appsolute/MAMP PRO/conf`.
     
*Postfix (main.cf)*
     
Open and edit your main.cnf template file here. There are likely several versions of MySQL available, each of them with      their own template file. Changes made to your template file will be reflected your real main.cnf file. The main.cnf         file created from the template file and is located in `/Library/appsolute/MAMP PRO/conf`.
     


---

#### Werkseinstellungen

##### Setting 1

Hiermit werden die Einstellungen aller virtuellen Hosts und die Servereinstellungen zurückgesetzt. Die Ports werden auf 8888, 8890 und 8889 zurückgesetzt, Apache- und MySQL-Benutzer auf username/username.

##### Setting 2

Hiermit werden die Einstellungen aller virtuellen Hosts und die Servereinstellungen zurückgesetzt. Der Apache-Port wird auf 80, 440 und 3306 zurückgesetzt, Apache- und MySQL-Benutzer auf www/mysql.

---

#### Backup…

Hiermit erstellen Sie ein Backup Ihrer Host-Einstellungen und Datenbankdateien. 

 

#### Aus Backup wiederherstellen…

Stellen Sie Ihre Host-Einstellungen und MySQL-Datenbankdateien aus einem Backup wieder her.

 
