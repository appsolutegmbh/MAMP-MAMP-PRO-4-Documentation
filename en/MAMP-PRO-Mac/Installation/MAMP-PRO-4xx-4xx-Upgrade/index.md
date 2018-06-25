---
title: MAMP PRO (Mac) Documentation > Upgrading from version 4.xx to version 4.xx
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Upgrading from version 4.xx to version 4.xx

1. Download MAMP PRO from [www.mamp.info](https://www.mamp.info){:target="_blank"}.
2. Double click on the `MAMP_MAMP_PRO_4.xx.pkg` file in your `Downloads` folder to start the installation process.
3. The installer will rename your existing `/Applications/MAMP` folder to `/Applications/MAMP_current_date`.
4. Your existing `htdocs` folder will be moved to your new `/Applications/MAMP` folder.
5. If there has been a change to the configuration of Apache, PHP, or MySQL (A directive was modified or a new one added)    between versions of MAMP PRO and you have already made changes to your current configuration (resulting in the creation of a template file in ~/Library/application support/appsolute/MAMP PRO/templates ), MAMP PRO will ask you to save off your old templates when you upgrade.

    ![MAMP](/en/MAMP-PRO-Mac/Installation/MAMP-PRO-4xx-4xx-Upgrade/Templates.png)
  
    Save your template files. You can use these saved template files as a guide of your previous modifications. New         (re) modifications need to be made through the MAMP PRO interface (File > Edit Templates), just as you had done previously in MAMP PRO.

6. Confirm that all data has been transferred correctly before starting MAMP PRO.
7. Your `/Applications/MAMP_current_date` folder can now be deleted. You may however keep it, so you can fall back to your original setup.

