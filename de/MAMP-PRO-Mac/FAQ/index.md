---
title: MAMP PRO (Mac) Dokumentation
description: 
layout: default-2
product: MAMP PRO Mac
language: de
---

## FAQ

### Was ist MAMP PRO?

MAMP PRO ist das kommerzielle, professionelle Konfigurationsprogramm für den Klassiker unter den lokalen Serverumgebungen: MAMP. MAMP PRO erlaubt Webentwicklern und Programmierern die komfortable Installation und Administration ihrer Entwicklungsumgebung unter OS X.

---

### Sind Updates kostenlos?

Innerhalb einer Hauptversion sind alle Updates kostenlos. Möchten Sie zum Beispiel MAMP PRO von Version 4.0 auf Version 4.xx aktualisieren, können Sie Ihre bisherige Seriennummer weiterverwenden.

---

### Ist MAMP PRO kompatibel mit Mac OS X 10.11 (El Capitan)?

Ja, MAMP PRO ist kompatibel mit Mac OS X 10.11 (El Capitan).

---

### Kann ich MAMP gleichzeitig mit MAMP PRO verwenden?

MAMP PRO ist ein Konfigurationswerkzeug für MAMP. Theoretisch könnten Sie MAMP parallel zu MAMP PRO benutzen, allerdings ist dies weder hilfreich, noch wird es von uns empfohlen, denn es kann zu vereinzelten Problemen mit Konfigurationsdateien - im schlimmsten Fall sogar zu Datenverlusten - führen.

---

### Welche PHP-Module sind enthalten?

Um herauszufinden, welche PHP-Module enthalten sind, klicken Sie auf den (i)-Button im Bereich Host -> Allgemein. Es öffnet sich eine Webseite u. a. mit Informationen zu installierten PHP-Modulen. Dazu muss der Server gestartet sein.

---

### Wo finde ich meine Registrierungsnummer?

Öffnen Sie den Dialog MAMP PRO -> Über MAMP PRO in der Menübar.

---

### Ist es möglich, eine aktualisierte Version von PHP hinzufügen?

Binaries des PHP-Interpreters können von https://www.mamp.info/en/downloads/ geladen werden. Verschieben Sie den herunter geladenen Ordner in das Verzeichnis /Programme/ MAMP/bin/php. Beenden Sie gegebenenfalls MAMP PRO und starten es erneut. Ihre neue PHP-Version sollte jetzt im Bereich PHP unter Standardversion im Dropdown-Menü erscheinen. MAMP PRO unterstützt ausschließlich PHP-Versionen von unserer Download-Seite.

---

### Kann MAMP PRO die selben Ports verwenden wie MAMP?

Ja, Sie können MAMP PRO die selben Ports zuweisen wie MAMP. Allerdings ist es nicht empfehlenswert, beide Programme (MAMP und MAMP PRO) zeitgleich laufen zu lassen.

---

### Where should I store my HTML and PHP pages?

By default, PHP and HTML Pages should be stored inside the MAMP /Applications/MAMP/htdocs folder. This folder is called "Document Root“. The location of the document root folder can be changed in the host settings.

---

### Ist das ImageMagick PHP-Modul enthalten?

Das ImageMagick PHP-Modul ist enthalten, aber nicht standardmäßig aktiviert. Sie müssen es mit Hilfe der Vorlagendatei php.ini editieren. Entfernen Sie dazu das ';' aus der Zeile ;extentsion=imagick.so.

---

### Welche Apache-Module sind enthalten?

Sie finden alle Apache-Module im Ordner /Programme/MAMP/Library/Module.

---

### Ist es möglich MAMP PRO auf einer externen Festplatte zu installieren?

Nein, MAMP PRO (und auch MAMP) muss auf dem Systemlaufwerk installiert werden.

---

### Will MAMP work if the MAMP folder is not located in the Applications directory?

No. In order to work properly the MAMP folder has to be located in the Applications folder.

---

### Ist die Anzahl der Aliase eines virtuellen Hosts begrenzt?

Nein, Sie können beliebig viele Aliase für einen virtuellen Hosts anlegen.

---

### Wo finde ich die Logs?

Klicken Sie auf den Rechtspfeil-Button, dann wird die Logdatei in der Konsole von OS X geöffnet.

---

### Welche Dateien werden von MAMP PRO auf meinem System erstellt oder verändert?

MAMP PRO versucht möglichst keine Dateien außerhalb des eigenen Programmverzeichnisses zu ändern. Die folgende Liste enthält alle Dateien, die durch MAMP PRO geändert werden und sich nicht innerhalb des MAMP PRO Ordners befinden:

MAMP PRO Einstellungen

/Library/Application Support/appsolute/MAMP PRO
~/Library/Application Support/appsolute/MAMP PRO
~/Library/Peferences/de.appsolute.mamppro.plist
Dynamisches DNS

/Library/LaunchDaemons/de.appsolute.mamp_dyndns.plist
~/Library/LaunchAgents/de.appsolute.mamp_dyndns.plist
Autostart bei Systemstart

/Library/StartupItems/MAMP/MAMP
/Library/StartupItems/MAMP/StartupParameters.plist
Postfix

Bevor eine neue Konfigurationsdatei erstellt wird, wird - falls vorhanden - eine postfix-Konfiguration unter /etc/postfix/MAMP_backup gesichert.

