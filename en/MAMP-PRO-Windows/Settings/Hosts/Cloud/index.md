---
title: MAMP PRO (Windows) Documentation > Settings > Hosts > Cloud
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Settings > Hosts > Cloud

Hosts can be saved to and loaded from the cloud. MAMP PRO will save both your document root folder and database data. Your data for each individual host will be saved in a single zip file in your Dropbox. It is not necessary to install Dropbox software to use this feature, you only need a login to your Dropbox account through the MAMP PRO interface [cloud settings](../../Cloud). 

If you have a data driven host, you must first associate the database with the host before you save it to the cloud. Associating a host with a database can be done on the [Databases tab](../Databases). Hosts using Extras or the WordPress host installation automatically have their databases associated with the host.

![MAMP](/en/MAMP-PRO-Windows/Settings/Hosts/Cloud/cloudhost.png)

---

* **Last Save to Cloud**

  The date of your last save to cloud.

* **Last Load from Cloud**

  The date of your last load to cloud.

* **Cloud space used**

  Your available cloud space from your cloud provider. 

---

### Cloud Functions

*  **Save to cloud**

    When saving to the cloud, MAMP PRO archives the data from the hosts document root folder and data from the MySQL databases and tables mapped to the host into a single zip file and optionally encrypts it with your encryption key. The archive will be transferred to the cloud afterwords. When encryption is used your archive is saved with a .encryptedzip extension.

*  **Load from cloud**

    Loading data from the cloud is the reverse process: After having loaded the archive, it will be decrypted if necessary, decompressed and the data will be copied to the hosts document root folder and imported back into MySQL. 

*  **Delete from cloud**

    Delete cloud data for a host.   
    
*  **Resolve name change**

    You may change the name of your host that is linked to the cloud. When you change the name of your linked host, the new host name must be resolved on all other linked machines.
    
    For instance, when you change a host name from "MyHost2" to "MyHost3", your Dropbox will modify it's stored zip file name from "MyHost2.zip" to "MyHost3.zip". You will then receive the following warning on your other linked computers indicating the host name has been changed in the cloud.
    
---
   
### Desktop Functions
   
  *  **Save To Desktop**
  
      This function will save an archive to your desktop. This can help you view what will get transferred, before sending data to the cloud, or determine how much free space you will need in the cloud.
  
  *  **Load To Desktop**
  
      This function will save a decrypted and uncompressed archive to the desktop. This can be useful if you want to peek into the data that is currently stored in the clould for the selected host. 
