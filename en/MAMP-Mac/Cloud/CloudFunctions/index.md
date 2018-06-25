---
title: MAMP (Mac) Documentation > Cloud Functions
description: 
layout: default-2
product: MAMP Mac
language: en
---

## Cloud Functions

You can "Save To Cloud" and "Load From Cloud" using the cloud functions.

![MAMP](/en/MAMP-Mac/Cloud/CloudSaveLoad.png)

---

### Cloud Status

Indicates whether your cloud functions are on or off.

### Document Root

The document root of your localhost, which will be saved to and loaded from the cloud.

### Database

The database associated with your localhost (optional).

---

### Save to Cloud

After you log into Dropbox and choose your settings you can save your host data to the cloud. Press "Save to cloud" to begin the process. Your data consists of a zip file containing your document root files and database data. You data will be saved to the cloud. If you have the Dropbox app you will also see your data in `/Dropbox/Apps/MAMP.`.

![MAMP](/en/MAMP-Mac/Cloud/CloudSaveToCloud.png)

### Load from Cloud

Your data will be loaded from the cloud. If you have the Dropbox application installed, you will also see it appear in `/Dropbox/Apps/MAMP.`.

![MAMP](/en/MAMP-Mac/Cloud/CloudLoading.png)

A backup of your local data will be made first when you load data from the cloud. You can delete this backup if you have successfully loaded from the cloud.

![MAMP](/en/MAMP-Mac/Cloud/backups.png)

---

<div class="alert" role="alert">
Note: Your files will not be synced automatically, you must manually load an store your hosts using the load and store commands from the menu.
</div>


### Before transferring data to the cloud : Always encrypt the data
  
  Use this feature to encrypt your data before moving it to Dropbox. You can encrypt all data before transferring it to the cloud, using the Advanced Encryption Standard (AES) and an encryption key you provide. The key will be stored in the systems keychain. You cannot set the encryption key if there is cloud activity.
  
  <div class="alert" role="alert">
  When you set encryption your files will be stored on Dropbox with a .encryptedzip extension. Previously stored hosts will keep their .zip, unencrypted extension, until the are reloaded to the cloud.
  </div>
  

