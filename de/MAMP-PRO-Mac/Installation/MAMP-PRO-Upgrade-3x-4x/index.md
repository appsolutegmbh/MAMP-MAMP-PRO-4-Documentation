---
title: MAMP PRO (Mac) Dokumentation
description: 
layout: default-2
product: MAMP PRO Mac
language: de
---

## Update von MAMP PRO 3 auf MAMP PRO 4

1. Laden Sie MAMP PRO von unserer Webseite https://www.mamp.info herunter.
2. Öffnen Sie die geladene Datei MAMP_MAMP_PRO_4.0.pkg per Doppelklick
3. Falls Sich bereits eine Version von MAMP auf ihrem Rechner befindet:
    Ein bereits vorhandener MAMP-Ordner wird in MAMP_aktuelles_Datum umbenannt.
    Ein bereits vorhandener htdocs-Ordner wird in den neuen Ordner `/Programme/MAMP` verschoben.
4. Überprüfen Sie, ob alle Dateien korrekt verschoben wurden, bevor Sie MAMP PRO starten.
5. Der Ordner `/Programme/MAMP_aktuelles_Datum` kann gelöscht werden. Sie können ihn aber auch behalten, falls Sie zu einem     späteren Zeitpunkt noch einmal darauf zugreifen möchten.
6. If you were using MySQL 5.5 (most likely scenerio) you will be informed to upgrade your MySQL to 5.6 . This is         recommended. Your original database data has been copied from `/Library/Application Support/appsolute/MAMP PRO/db/mysql` to `/Library/Application Support/appsolute/MAMP PRO/db/msql56`. 

![MAMP](UpgradeMySQLNotice.png)
 
7. When the installation process is finished and you open MAMP PRO for the first time you prompted to upgrade your databases to MySQL 5.6. Click Upgrade to upgrade your databases. 

![MAMP](UpgradeMySQL.png)

8. The installation process will create an `/Applications/MAMP_current_date` folder. This folder can now be deleted. You may however keep it, so you can fall back to your original setup.
