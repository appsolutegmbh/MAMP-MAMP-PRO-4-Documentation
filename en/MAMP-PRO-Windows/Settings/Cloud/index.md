---
title: MAMP PRO (Windows) Documentation > Settings > Cloud
description: 
layout: default-2
product: MAMP PRO Windows
language: en
lastedit: 2021-03-26
---

## Settings > Cloud

Store and load your host and database data using a cloud provider. Currently Dropbox is available for this option. It is not necessary to install Dropbox software to use this feature, you only need a Dropbox account. After you log into Dropbox and choose your settings you can save and load your hosts using the functionality in the hosts table. More information on your using host cloud functions can be found [here](../Hosts/Cloud). 


<div class="alert" role="alert">
Note: Your files will not be synced automatically, you must manually load and store your hosts using the load and store functions.
</div>

![MAMP](/en/MAMP-PRO-Windows/Settings/Cloud/cloud.PNG)

---

### Use Cloud Service

When you check this option you will be asked to log into your Dropbox account. When you have completed the login process your Dropbox will be linked to MAMP PRO. When saving to cloud it will be saved as either a zip archive (.zip) or an encrypted zip archive (.encryptedzip), depending on the encryption settings. 

![MAMP](/en/MAMP-PRO-Windows/Settings/Cloud/dropbox.PNG)

---

### Before transferring data to the cloud : Always encrypt the data
  
  Use this feature to encrypt your data before moving it to Dropbox. You can encrypt all data before transferring it to the cloud, using the Advanced Encryption Standard (AES) and an encryption key you provide. The key will be stored in the systems keychain. You cannot set the encryption key if there is cloud activity.
  
  <div class="alert" role="alert">
  When you set encryption your files will be stored on Dropbox with a .encryptedzip extension. Previously stored hosts will keep their .zip, unencrypted extension, until the are reloaded to the cloud.
  </div>
  
### Unattended transfers : Prevent sleeping during cloud activity
  
If there is cloud activity MAMP PRO can prevent your computer from going into sleep mode. After all cloud activity has been finished MAMP PRO no longer prevents sleep mode.
  
---

### Path to log file
 
 The path to your cloud log file. Your cloud activity log is located in "C:\Mamp\logs".
 
---

### Cloud Activity

When saving to cloud it will be saved as either a zip archive (.zip) or an encrypted zip archive (.encryptedzip), depending on the encryption settings. This file will be transferred directly to Dropbox. If you have the Dropbox software installed and the MAMP PRO folder is not in the exception list, the Dropbox software will download the folder content to "C:\Users\UserName\Dropbox\Apps\MAMP PRO" after MAMP PRO has uploaded data. 

When MAMP PRO turns off the Cloud activity signals the data has been completely transferred to Dropbox. At that point, the Dropbox software might not even have started to re-transfer the data back to the originating computer. The Dropbox is not an indicator that MAMP PRO has finished its cloud work.

The "transmission" entry next to the cloud icon on the sidebar shows you if MAMP Pro is finished with its cloud work.

![MAMP](/en/MAMP-PRO-Windows/Settings/Cloud/sidebar.PNG)