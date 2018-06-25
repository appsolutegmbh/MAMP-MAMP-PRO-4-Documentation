---
title: MAMP PRO (Mac) Dokumentation
description: 
layout: default-2
product: MAMP PRO Mac
language: de
---

#### Update von MAMP PRO 4.xx auf MAMP PRO 4.xx

1. Laden Sie MAMP PRO von unserer Webseite https://www.mamp.info herunter.
2. Öffnen Sie die geladene Datei MAMP_MAMP_PRO_4.0.pkg per Doppelklick
3. Das Installationsprogramm wird Sie durch den Installationsprozess führen.
4. Falls Sich bereits eine Version von MAMP auf ihrem Rechner befindet:
    Ein bereits vorhandener MAMP-Ordner wird in MAMP_aktuelles_Datum umbenannt.
    Ein bereits vorhandener htdocs-Ordner wird in den neuen Ordner `/Programme/MAMP` verschoben.
5. If there has been a change to the configuration of Apache, PHP, or MySQL (A directive was modified or a new one added)    between versions of MAMP PRO and you have already made changes to your current configuration (resulting in the creation of a template file in ~/Library/application support/appsolute/MAMP PRO/templates ), MAMP PRO will ask you to save off your old templates when you upgrade.

    ![MAMP](Templates.png)
  
    Save your template files. You can use these saved template files as a guide of your previous modifications. New         (re) modifications need to be made through the MAMP PRO interface (File > Edit Templates), just as you had done before in your previous version of MAMP PRO.

6. Confirm that all data has been transferred correctly before starting MAMP PRO.
7. Your `/Applications/MAMP_current_date` folder can now be deleted. You may however keep it, so you can fall back to your original setup.

