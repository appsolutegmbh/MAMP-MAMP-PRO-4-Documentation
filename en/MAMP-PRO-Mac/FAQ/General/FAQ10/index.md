---
title: MAMP PRO (Mac) Documentation > FAQ > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Where exactly are the MAMP PRO files created or changed?

The following list contains all files which are created and changed by MAMP PRO and are not located within the MAMP PRO folder.

*  **MAMP PRO Settings and Files**  
    * /Library/Application Support/appsolute/MAMP PRO
    * ~/Library/Application Support/appsolute/MAMP PRO
    * ~/Library/Preferences/de.appsolute.mamppro.plist 
    * ~/Library/Preferences/de.living-e_to_appsolute.mampro.plist
    * ~/Library/Preferences/de.appsolute.MAMP.plist
  
*  **MySQL**  
    * /Library/Application Support/appsolute/MAMP PRO/db/mysql  
  
*  **Dynamic DNS**  
    * /Library/LaunchDaemons/de.appsolute.mamp_dyndns.plist
    * ~/Library/LaunchAgents/de.appsolute.mamp_dyndns.plist  
  
*  **Autostart at system start**  
    * /Library/StartupItems/MAMP/MAMP
    * /Library/StartupItems/MAMP/StartupParameters.plist  
  
*  **Postfix**  
    * An existing postfix configuration will be backed up to `/etc/postfix/MAMP_backup` before writing a new config file.  


