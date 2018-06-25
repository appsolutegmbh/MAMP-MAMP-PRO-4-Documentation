---
title: MAMP PRO (Mac) Dokumentation
description: 
layout: default-2
product: MAMP PRO Mac
language: de
---

## Troubleshooting

### Beim letzten Öffnen der Extras gab es ein Content Management System welches jetzt nicht mehr verfügbar ist?

Dies kann verschiedene Gründe haben:

Bitte überprüfen Sie zunächst Ihre Internetverbindung. Ohne Internetverbindung zeigt MAMP PRO nur Extras an, die Sie zuvor installiert haben.
Es kann auch sein, dass ein Extra nicht angezeigt wird, weil die für den virtuellen Host gewählte PHP-Version nicht kompatibel mit dem Extra ist.
Eventuell haben Sie zu wenig freien Speicherplatz auf Ihrer Festplatte.
Manche Extras können auf einem virtuellem Host nur einmal installiert werden. Dies ist beispielsweise bei dem Extra webEdition der Fall.

---

### Ich habe Wordpress installiert und werde nach meinem Benutzernamen und Passwort gefragt?

Nach der Installation von Wordpress lautet Ihr Benutzername/Passwort: admin/admin.

---

### Der Apache-Server startet nicht

Das häufigste Problem bei einem Apache-Server der nicht startet, ist eine weitere Apache-Instanz, die bereits auf dem selben Port läuft. Um dies zu überprüfen gehen Sie wie folgt vor:

1. Beenden Sie MAMP PRO. 

2. Öffnen Sie den Aktivitätsmonitor im Ordner /Programme/Dienstprogramme. 

3. Geben Sie httpd in das Suchfeld oben rechts ein.

4. Beenden Sie jeden Prozess, den Sie nach Ihrer Suche finden. 

5. Starten Sie MAMP PRO. 

Wenn der Apache-Server immer noch nicht startet, überprüfen Sie die Protokolldatei auf Fehlermeldungen.

---

### Changes to my php.ini file and/or my httpd.conf file are not showing up when I restart MAMP PRO.

You must edit the httpd.conf, php.ini and my.cnf files through the Template Editor provided by MAMP PRO. Go to File->Edit Template to edit template files.

---

### Der MySQL-Server startet nicht

Das häufigste Problem bei einem MySQL-Server der nicht startet, ist ein weiterer MySQL-Dienst, der auf dem selben Port läuft. Um dies zu überprüfen gehen Sie wie folgt vor:

1. Beenden Sie MAMP PRO. 

2. Öffnen Sie den Aktivitätsmonitor im Ordner /Programme/Dienstprogramme. 

3. Geben Sie mysqld in das Suchfeld oben rechts ein.

4. Beenden Sie jeden Prozess, den Sie nach Ihrer Suche finden. 

5. Starten Sie MAMP PRO. 

Sollte MySQL immer noch nicht starten, überprüfen Sie die Protokolldatei auf Fehlermeldungen.

 



