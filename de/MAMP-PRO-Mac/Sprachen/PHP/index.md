---
title: MAMP PRO (Mac) Dokumentation
description: 
layout: default-2
product: MAMP PRO Mac
language: de
---

## Sprachen > PHP

PHP ist eine weit verbreitete Web-Scripting Programmiersprache. MAMP PRO installiert mehrere Versionen der PHP-Skript-Interpreter.

![MAMP](php.png)

---

*  **Standardversion**  
   Wählen Sie die PHP-Version aus, die Sie als Standard verwenden möchten. Diese Version wird  dann für alle Hosts              verwendet, solange Sie sich in der Betriebsart Modul (siehe folgenden Abschnitt) befinden.

   *  **Make this version also available on the command line** 
      Your command line will now automatically point to the version of php in your MAMP PRO.

---

*  **Betriebsart**  
   Sie können zwischen zwei Betriebsarten wählen:

   *  **Modul-Modus (Gleiche PHP Version für alle Hosts)**
   *  **CGI-Modus (Individuelle PHP-Version für jeden Host)**

   Im Modul-Modus verwendet jeder Host die PHP-Version, die Sie als Standardversion eingestellt haben. Wechseln sie die         PHP-Standard-Version, gilt diese Einstellung automatisch für alle Hosts. Im CGI-Modus können Sie jedem Host eine             individuelle PHP-Version zuweisen (Reiter Hosts). Informationen dazu finden Sie im Abschnitt 2. Hosts.
   
---

*  **Cache-Modul zum Beschleunigen der PHP-Ausführung**  
   PHP verfügt über mehrere Cache-Erweiterungen, die zu einer beschleunigten Ausführung ihrer Webseite führen können.      Standardmäßig ist das Caching abgeschaltet. Eine Aktivierung des Cache-Moduls führt nicht zwangsläufig zu einer höheren Ausführungsgeschwindigkeit.

   *  **off**  
   *  **APC**  
   *  **eAccelerator**  
   *  **XCache**  
   *  **OPCache**  
   
![MAMP](cache.png) 
   
Several caches provide a user interface to help analyze and profile your code. Press the Arrow button to the right of the  cache name to view this interface. An interface is not available if the Arrow button is not enabled.

---

*  **Xdebug aktivieren**  
   Aktivieren Sie Xdebug, um PHP-Debugging Informationen während der Skriptausführung zu erhalten. Standardmäßig verwendet      Xdebug zur Kommunikation mit externen Debuggern localhost und Port 9000 in der php.ini-Datei.

*  **MacGDP starten**  
   Bei aktiviertem Xdebug können Sie den MacGDBp-Debugger öffnen, um ein PHP-Debugging zu starten. Standardmäßig erwartet       MacGDBp Debugging-Informationen auf Port 9000 von localhost. Siehe http://www.bluestatic.org/software/macgdbp/ für weitere    Informationen. 

---

*  **Zu protokollierende Fehler**  
   Hier legen Sie fest, was während der Ausführung eines Scripts protokolliert werden soll:

   Fehler anzeigen, die beim Start von PHP auftreten: Zeichnet PHP-Fehler auf, die auftreten, wenn Apache das PHP-Module       lädt.

   Alle Fehler und Warnungen: Alle Fehler werden aufgezeichnet.

   Fehler: Skriptfehler, die eine weitere Ausführung eines aktuellen PHP-Scripts unmöglich machen, werden aufgezeichnet.

   Warnungen: Allgemeine Fehler in der PHP-Umgebung werden aufgezeichnet.

   Hinweise: Mögliche Probleme die PHP nicht unbedingt behindern, die aber ein Hinweis auf einen Fehler in einem Skript sein    könnten, werden aufgezeichnet.

   Andere: Über spezielle, vordefinierte Konstante können Sie hier weitere Fehlertypen aufzeichnen lassen. Mehr Informationen    finden Sie in der Dokumentation von PHP.
 
---
   

*  **Fehlerprotokoll**  
   Hier legen Sie fest, ob das Fehlerprotokoll auf dem Bildschirm angezeigt und/oder in einer Logdatei protokolliert werden     soll. Den Speicherort dieser Datei dürfen Sie frei wählen.
   
