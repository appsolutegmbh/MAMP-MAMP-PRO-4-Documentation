---
title: MAMP (Mac) Dokumentation - Anleitungen
description: Anleitungen
layout: default-2
product: MAMP Mac
language: de
---

## Anleitungen

### Upgrade Data from MySQL 5.5 to MySQL 5.6

Your current MySQL 5.5. data is located in `/Applications/MAMP/db/mysql`.
You need to export your data first. You can use mysqldump to export your data. To do this cut and paste the following in a terminal window.

`/Applications/MAMP/Library/bin/./mysqldump -u root -p --all-databases > /Applications/MAMP/db/dump.sql`

You will be prompted for your MySQL root user password. By defualt MAMP PRO sets this to [root].
After you have entered your password you should have a dump.sql file in your /Applications/MAMP/db folder


### Wie ändere ich das Passwort für den MySQL-Benutzer root?

Öffnen Sie das Programm Terminal (in "/Programme/Dienstprogramme") und geben Sie die folgenden Zeilen ein:


`cd /Programme/MAMP/Library/bin./mysqladmin -u root -p password <NEWPASSWORD>`
Schließen Sie beide Zeilen mit Enter ab. Ersetzen Sie <NEWPASSWORD> mit dem neuen Passwort.

Hinweis
Bitte beachten Sie, dass Sie das neue Passwort auch in der phpMyAdmin-Konfiguration in `/Programme/MAMP/bin/phpMyAdmin/config.inc.php` eintragen müssen, und auch in Ihren eigenen Skripten, die mit MySQL zusammenarbeiten.

---

### Default Storage Engine von MySQL herausfinden

Öffnen Sie MAMP.
Starten Sie die Server
Öffnen Sie das Terminal.app (Programme -> Dienstprogramme).
Geben Sie folgenden Befehl ein und bestätigen Sie mit Enter:
`cd /Programme/MAMP/Library/bin`
Geben Sie folgenden Befehl ein und bestätigen Sie mit Enter
`./mysql --host=localhost -u root -proot`
Geben Sie folgenden Befehl in der Eingabeaufforderung von MySQL (mysql>) ein und bestätigen Sie mit Enter:
`USE information_schema;`
Geben Sie folgenden Befehl in der Eingabeaufforderung von MySQL (mysql>) ein und bestätigen Sie mit Enter:
`SELECT * FROM engines;`
Es wird eine Tabelle mit den Storage Engines des MySQL-Server angezeigt. In der Spalte SUPPORT steht bei Default Storage Engine der Wert DEFAULT.


Geben Sie folgenden Befehl in der Eingabeaufforderung von MySQL (mysql>) ein und bestätigen Sie mit Enter:
`exit;`

---

### Default Storage Engine von MySQL einstellen

Der MySQL-Server von MAMP nutzt die Default Storage Engine MyISAM. Möchten Sie dies ändern, müssen Sie die Konfigurationsdatei des MySQL-Servers erweitern. Die folgende Anleitung zeigt, wie Sie die Default Storage Engine auf InnoDB setzen.

Stoppen Sie die MAMP-Server, falls diese aktiv sind.
Erstellen Sie mit einem geeigneten Texteditor (etwa TextWrangler von BareBones.com) eine Datei namens my.cnf und sichern Sie diese im Verzeichnis `/Programme/MAMP/conf/`.
Fügen folgenden Inhalt in diese Datei ein:
 `[mysqld]default-storage-engine = InnoDB`
Speichern Sie die Datei my.cnf und schließen Sie den Texteditor.
Starten Sie die MAMP-Server.

<div class="alert" role="alert">
Hinweis: Speichern Sie als reine Textdatei (Endung txt), nicht im Word- oder RTF-Format.
</div>

---

### MySQL über die Kommandozeile nutzen

Um auf den MySQL-Server über die Kommandozeile zuzugreifen, gehen Sie wie folgt vor:

Öffnen Sie MAMP
Starten Sie die Server
Öffnen Sie das Terminal (Programme -> Dienstprogramme)
Geben Sie Folgendes ein und bestätigen Sie mit Enter
`cd /Programme/MAMP/Library/bin`
Geben Sie danach das Folgende und bestätigen Sie wieder mit Enter
`./mysql --host=localhost =u root -proot`
Nun kann man sich zum Beispiel mit `show databases;` die angelegten Datenbanken anzeigen lassen.
`show databases;`

---

### MySQL-Datenbankverbindung (mysqli)

Das folgende Beispiel zeigt, wie man in PHP mittels der Funktion mysqli() eine Verbindung zu einer MySQL-Datenbank herstellt:

`php
 DEFINE('DB_USER', 'root');
 DEFINE('DB_PASSWORD', 'root');
 DEFINE('DB_HOST', 'localhost');
 DEFINE('DB_DATABASE', 'performance_schema');

 // siehe auch http://www.php.net/manual/en/mysqli.connect.php
 $mysqli = new mysqli(DB_HOST, DB_USER, DB_PASSWORD, DB_DATABASE);

 if (mysqli_connect_error()) {
  die('Connect Error (' . mysqli_connect_errno() . ') ' . mysqli_connect_error());
 }

 echo 'Connected successfully.’;

 $mysqli->close();
?>`

---

<a name="upgrade_to_mamp_pro_missing_databases"></a>

### How To Transfer Your Databases From MAMP To MAMP PRO 

1. Stop your servers and close any instances of MAMP and MAMP PRO.
2. Open your Mac Finder and navigate to `/Library/application data/appsolute/MAMP PRO`.
3. Rename your `/db` folder to `/db_bak`.
4. Open MAMP PRO and launch your servers.

When MAMP PRO launched it's servers it (re) copied database data from the MAMP location to the MAMP PRO location because it did not detect a `/Library/application data/appsolute/MAMP PRO/db` folder. You should now be looking at your current database data.




