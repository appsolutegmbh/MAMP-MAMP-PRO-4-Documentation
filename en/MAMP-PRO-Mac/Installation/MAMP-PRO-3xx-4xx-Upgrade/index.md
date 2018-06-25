---
title: MAMP PRO (Mac) Documentation > MAMP PRO 3.xx to 4.xx Upgrade
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## MAMP PRO 3.xx to 4.xx Upgrade

When upgrading to MAMP PRO 4 you will be asked to upgrade your data to MySQL 5.6 This is recommended. Your current MySQL data will be copied from `/Library/Application Support/appsolute/MAMP PRO/db/mysql` to  `/Library/Application Support/appsolute/MAMP PRO/db/mysql56`. Your old data will be preserved intact in  `/Library/Application Support/appsolute/MAMP PRO/db/mysql`.

1. Download MAMP PRO from [www.mamp.info](https://www.mamp.info){:target="_blank"} .
2. Double click on the `MAMP_MAMP_PRO_4.xx.pkg` file in your `Downloads` folder to start the installation process.
3. The installer will rename your existing `/Applications/MAMP` to `/Applications/MAMP_current_date`. This folder can later be deleted. You may however keep it, so you can fall back to your original setup.
4. Your existing `htdocs` folder will be moved to your new `/Applications/MAMP` folder.
5. Confirm that all data has been transferred correctly before starting MAMP PRO.
6. If you were using MySQL 5.5 (most likely scenerio) you will be informed of the upgrade to MySQL 5.6 . 

![MAMP](/en/MAMP-PRO-Mac/Installation/MAMP-PRO-3xx-4xx-Upgrade/UpgradeMySQLNotice.png)

When you open MAMP PRO and start your servers for the first time you will be prompted to upgrade your database data to MySQL 5.6. Click OK to proceed with the database upgrade. 

![MAMP](/en/MAMP-PRO-Mac/Installation/MAMP-PRO-3xx-4xx-Upgrade/UpgradeInfo.png)

Click on Upgrade to upgrade your databases to 5.6

![MAMP](/en/MAMP-PRO-Mac/Installation/MAMP-PRO-3xx-4xx-Upgrade/UpgradeDatabases.png)

---

<i class="fa fa-play-circle-o fa-lg" aria-hidden="true"></i> [Upgrading From MAMP PRO 3 To MAMP PRO 4](https://www.youtube.com/watch?v=OoBnH29AAi8){:target="_blank"}
