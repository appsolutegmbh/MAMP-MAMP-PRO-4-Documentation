---
title: MAMP PRO (Mac) Documentation > Settings > Cloud
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Settings > Cloud

Store and load your host and database data using a cloud provider. Currently Dropbox is available for this option. It is not necessary to install Dropbox software to use this feature, you only need a Dropbox account. After you log into Dropbox and choose your settings you can save and load your hosts using the functionality in the hosts table. More information on your host cloud functions can be found [here](../Hosts/Cloud). 


<div class="alert" role="alert">
Note: Your files will not be synced automatically, you must manually load, store and link your hosts using the load, store, and link commands from the menu.
</div>

![MAMP](/en/MAMP-PRO-Mac/Settings/Cloud/cloud.png)

---

### Use Cloud Service

When you check this option you will be asked to log into your Dropbox account. When you have completed the login process your Dropbox will be linked to MAMP PRO. When saving to cloud it will be saved as either a zip archive (.zip) or an encrypted zip archive (.encryptedzip), depending on the encryption settings. You need to individually link each host to Dropbox. 

![MAMP](/en/MAMP-PRO-Mac/Settings/Cloud/dropbox.png)

---

### Before transferring data to the cloud : Always encrypt the data
  
  Use this feature to encrypt your data before moving it to Dropbox. You can encrypt all data before transferring it to the cloud, using the Advanced Encryption Standard (AES) and an encryption key you provide. The key will be stored in the systems keychain. You cannot set the encryption key if there is cloud activity.
  
  <div class="alert" role="alert">
  When you set encryption your files will be stored on Dropbox with a .encryptedzip extension. Previously stored hosts will keep their .zip, unencrypted extension, until the are reloaded to the cloud.
  </div>
  
### When authorizing MAMP PRO with Dropbox : Use in-app webview
  
  If your default web browser is not set to Safari you may experience trouble authorizing MAMP PRO with Dropbox or  switching accounts. Temporarily switching to Safari as your default browser or temporarily activating this option remedies these problems. 
  
### Unattended transfers : Prevent sleeping during cloud activity
  
  If there is cloud activity MAMP PRO can prevent your computer from going into sleep mode. After all cloud activity has been finished MAMP PRO no longer prevents sleep mode.
  
---
 
### Path to log file
 
 The path to your cloud log file. Your cloud activity log is located in `/Applications/MAMP PRO/logs`
 
---
 
### Cloud Activity

When saving to cloud it will be saved as either a zip archive (.zip) or an encrypted zip archive (.encryptedzip), depending on the encryption settings. This file will be transferred directly to Dropbox. If you have the Dropbox software installed and the MAMP PRO folder is not in the exception list, the Dropbox software will download the folder content to `~/Dropbox/Apps/MAMP PRO` after MAMP PRO has uploaded data. 

When MAMP PRO turns off the Cloud activity signals the data has been completely transferred to Dropbox. At that point, the Dropbox software might not even have started to re-transfer the data back to the originating computer. The Dropbox is not an indicator that MAMP PRO has finished its cloud work.

You can spot cloud related activity when you see the cloud logo in the toolbar and menubar are green. 

![MAMP](/en/MAMP-PRO-Mac/Settings/Cloud/menuBar.png)

![MAMP](/en/MAMP-PRO-Mac/Settings/Cloud/toolBar.png)







