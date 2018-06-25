---
title: MAMP PRO (Mac) Dokumentation - Anleitungen
description: 
layout: default-2
product: MAMP PRO Mac
language: de
---

## Anleitungen

### Output Buffering aktivieren

Starten Sie MAMP PRO
Wählen Sie aus dem Menü Ablage -> Vorlage Editieren den Menüpunkt PHP 5.5.x php.ini beziehungsweise PHP 5.5.x php.ini
 
Suchen Sie folgende Zeile: output_buffering = Off
Ändern Sie den Wert Off zu On oder die maximale Anzahl an Bytes (etwa 4096)
Speichern Sie die Datei
Starten Sie die Server

---

### Die Default Storage Engine von MySQL herausfinden

MAMP öffnen.
Server starten.
Terminal.app (Programme -> Dienstprogramme) öffnen.
Folgenden Befehl eingeben und mit der Enter-Taste bestätigen:
cd /Applications/MAMP/Library/bin
Mit der Enter-Taste bestätigen
./mysql --host=localhost -u root -proot
In der Eingabeaufforderung von MySQL (mysql>) folgenden Befehl eingeben und mit der Enter-Taste bestätigen:
USE information_schema;
In der Eingabeaufforderung von MySQL (mysql>) folgenden Befehl eingeben und mit der Enter-Taste bestätigen:
SELECT * FROM engines;
Es wird eine Tabelle mit den Storage Engines des MySQL-Servers angezeigt. In der Spalte SUPPORT steht der Wert der Default Storage Engine auf DEFAULT. 
In der Eingabeaufforderung von MySQL folgenden Befehl eingeben und mit der Enter-Taste bestätigen:
exit;

---

### PHP-Speicherlimit erhöhen

MAMP PRO starten
Server stoppen (falls sie gestartet wurden)
Über das Menü Ablage -> Vorlage editieren den Menüpunkt PHP 5.2.x php.ini beziehungsweise PHP 5.2.x php.ini auswählen

Es wird die ausgewählte php.ini-Datei geöffnet
Falls nun ein Dialog mit einer Warnung erscheint, diesen lesen und mit OK bestätigen
Suchen (Apfel + F) Sie nun nach memory_limit
Sie sollten folgende Zeile finden (alles in einer Zeile) 
memory_limit = 32M ; Maximum amount of memory a script may consume (8M)
Ändern Sie hier den Wert von 32M auf 64M oder mehr (z.B.128 MB).
Speichern (Apfel + S) Sie die php.ini-Datei ab.
Schließen (Apfel + W) Sie die php.ini-Datei.
Starten Sie die Server.

---

### Die Default Storage Engine von MySQL setzen

Als Default Storage Engine verwendet MAMP PRO für den MySQL-Server (wie jeder andere MySQL-Server auch) MyISAM.
Soll dies geändert werden, muss dazu die Konfigurationsdatei des MySQL-Servers erweitert werden. Die folgende Anleitung zeigt, wie man dies mit MAMP PRO handhabt:

Als Default Storage Engine setzen wird dabei InnoDB ein.

MAMP PRO starten
Server stoppen (falls sie bereits gestartet wurden)
Aus dem Menü Ablage -> Vorlage editieren den Eintrag MySQL my.cnf auswählen. 

Die Datei my.cnf wird in einem Editorfenster geöffnet.
Falls ein Dialog Warnung erscheint, diesen mit einem Klick auf den OK-Button bestätigen.
Den Abschnitt "[mysqld]" suchen.
Unter die letzte Zeile dieses Abschnitts folgende neue Zeile einfügen:
default-storage-engine = InnoDB
Der Abschnitt "[mysqld]" sieht nun so aus:


Die Änderungen an der Datei my.cnf über das Menü Ablage -> Speichern (oder über die Tastenkombination "Apfel + S") sichern.
Das Editorfenster über das Menü Ablage -> Schließen (oder über die Tastenkombination "Apfel + W") schließen.
Starten Sie die Server von MAMP PRO.

---

### Postfix log Datei anzeigen

Hinweis: Möchten Sie die Logdatei von Postfix mit einem Texteditor (z.B. TextWrangler) editieren, müssen Sie zunächst im Finder alle unsichtbaren Ordner und Dateien sichtbar machen. Erst danach können Sie die Logdatei mit einem Texteditor öffnen. Dazu gehen Sie wie folgt vor:
Öffnen Sie das Programm “Terminal.app" (/Programme/Dienstprogramme/Terminal.app)

Geben Sie folgenden Befehl ein und drücken Sie die Enter-Taste:


defaults write com.apple.finder AppleShowAllFiles -boolean true
Starten Sie den Finder neu, indem Sie folgenden Befehl eingaben und mit der Enter-Taste bestätigen:


Killall Finder
Öffnen Sie nun die Datei /private/var/log/mail.log mit ihrem Texteditor.

---
 
### Die Logdatei von Postfix anzeigen (Über die Konsole (empfohlen))

Öffnen Sie das Programm "Konsole.app" (/Programme/Dienstprogramme/Konsole.app).
Wählen Sie über das Menü Darstellung den Eintrag Protokollliste einblenden.
Öffnen Sie in der Protokollliste den Ordner DATEIEN.
Öffnen Sie in der Protokollliste den Ordner /private/var/log
Klicken Sie auf den Eintrag mail.log.
Auf der rechten Seite des Programmfensters wird nun der Inhalt der Postfix-Logdatei angezeigt.

---

### Show Postfix Logfile Using MySQL command line

Öffnen Sie das Programm “Terminal.app" (/Programme/Dienstprogramme/Terminal.app)
Geben Sie folgenden Befehl ein und drücken Sie die Enter-Taste:

tail -f /private/var/log/mail.log
Nun wird der Inhalt der Logdatei von Postfix im Terminal angezeigt. Sobald sich die Datei verändert (neue Einträge hinzukommen), wird auch die Anzeige im Terminal-Fenster aktualisiert.
Press "Ctrl + c" to stop the process.

---

### How do I install PEAR?

Open up a terminal and type the following 

$ echo "export PATH=/Applications/MAMP/bin/php/phpX.X.X/bin:$PATH" >> ~/.profile
Close your terminal session and open up another one. Type the following in the terminal window

$ which PHP
You should see a path to one of your PHP installations.

Type the following in the terminal window

$ pear

---

### MySQL über die Kommandozeile nutzen

Möchten Sie über die Kommandozeile auf den MySQL-Server zugreifen, gehen Sie wie folgt vor:

 

1. Starten Sie MAMP PRO

2. Starten Sie die Server

3. Öffnen Sie das Terminal (Programme -> Dienstprogramme)

4. Geben Sie folgendes in das Terminal ein (alles in einer Zeile) und bestätigen Sie mit der Enter-Taste:

/Applications/MAMP/Library/bin/mysql --host=localhost -uroot -proot

 

Nun können Sie sich zum Beispiel mit show databases; die angelegten Datenbanken anzeigen lassen.

 


