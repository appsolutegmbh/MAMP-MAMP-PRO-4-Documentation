---
title: MAMP PRO (Mac) Documentation > First Steps
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## First Steps

![MAMP](/en/MAMP-PRO-Mac/First-Steps/FirstSteps.png)

When the MAMP PRO application is launched for the first time its helper tools will be installed. You will be prompted to enter your admin password.

Click on the Servers button in the title bar to launch Apache and MySQL, they are your default GroupStart web and database servers. The launch status of the server is displayed in the Servers & Services section. A check mark next to the server/service indicates that this server/service will start/stop when the Servers button is pressed.  The Apache web server (default web server) uses port 8888 by default. This port must be specified when calling the local web page in the browser, e.g.: http://localhost:8888

Your default host for MAMP PRO is `localhost`. The files for localhost are initially located in the `/Applications/MAMP/htdocs` folder. Press ![MAMP](/en/MAMP-PRO-Mac/First-Steps/BlackArrow.png) located to the right of the Name text box to open up the localhost in a web browser.

![MAMP](/en/MAMP-PRO-Mac/First-Steps/OpenLocalHost.png)

<div class="alert" role="alert">
Note: Although the default localhost document root is located in `/Applications/MAMP/htdocs`, it is best to keep it's document root, and the document root of additional hosts out of the `/Applications/MAMP folder`. A better directory structure for your host document root folders would be `~/sites/localhost`, `~/sites/site1`, `~/sites/site2`, etc ... .
</div>

---

### Add Additional Hosts

To add an additional host press the '+' button at the bottom left corner of the Hosts table. You will then be asked to select a document root folder and optionally a database. See the [Hosts](../Settings/Hosts/General) section for more information on what a host is and how to create additional hosts.

---

### Link To Cloud

You can link your new host to the cloud using a cloud provider. The following additional steps will link your host to the cloud.

1. In the sidebar switch to the "Cloud" section and activate "Use Cloud service". You will be transferred to the Dropbox site to provide your account credentials. Allow "MAMP PRO" to access its folders on Dropbox and switch back to the software.
2. Switch back to the "Hosts" section using the sidebar.
3. Enlarge the hosts table by clicking on the right-arrow on the lower-right corner of the table. You are now able to see the status messages.
4. Choose "Save to Cloud" from the contextual menu (right-click or ctrl-click) of the host you created in step 4. A zip archive will be transferred to Dropbox which can be downloaded on the same or a second machine by using "Load from Cloud" from the contextual menu. On the second machine the host must have the same name and you must "Link to Cloud" first.

See the [Dropbox](../Settings/Hosts/Cloud) section for more information on storing your hosts in the cloud.

---

### Main GUI Elements


*  **Customize**  
   Customize your toolbar. Additional information about the toolbar can be found in the [Customize](../Customize/) section.
*  **MAMP PRO**  
   Open the  [https://mamp.info](https://www.mamp.info){:target="_blank"} web page.
*  **Editor**  
   Open the MAMP PRO Editor. Additional information about the MAMP PRO Editor can be found in the [Editor](../Editor/)
   section.
*  **WebStart**  
   Open the MAMP PRO start page of your local web server.
   Additional information about the MAMP PRO start page is in the [Webstart](../WebStart) section.
*  **Servers**  
   Starts the current GroupStart services of MAMP PRO. Stops all services if any GroupStart services are already running. 
*  **Revert**  
   Discards all changes, which have not already been confirmed with `Save`.
*  **Save**  
   Save your changed settings.
*  **Server & Services**  
   'On' indicates a server or service is on, '-' indicates the service is off. A checkmark indicates this service is part of
   'Groupstart'.
   
   ![MAMP](/en/MAMP-PRO-Mac/First-Steps/ServerServices.png)

---

### Meaning of Icons

![MAMP](/en/MAMP-PRO-Mac/First-Steps/Docs.png) Change a file location, including the location of the document root, or a log file. 

![MAMP](/en/MAMP-PRO-Mac/First-Steps/Mail.png) Prepare an e-mail with the Xip.io URL of a host.

![MAMP](/en/MAMP-PRO-Mac/First-Steps/Rights.png) Modify the access rights of a document root folder.

![MAMP](/en/MAMP-PRO-Mac/First-Steps/BlackArrow.png) Open a disk location in the Finder, or a host in the web browser.

![MAMP](/en/MAMP-PRO-Mac/First-Steps/info.png) Provide more information, including phpInfo().

![MAMP](/en/MAMP-PRO-Mac/First-Steps/RedArrow.png) Indicates that information is missing.

![MAMP](/en/MAMP-PRO-Mac/First-Steps/Plus.png) Add a new PHP version.
