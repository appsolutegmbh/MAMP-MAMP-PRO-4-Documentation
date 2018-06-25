---
title: MAMP PRO (Windows) Documentation > First Steps
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## First Steps

![MAMP](/en/MAMP-PRO-Windows/First-Steps/FirstSteps.png)

Click on the Start button on the title bar to launch your Apache and MySQL, they are your default GroupStart web and database servers. The launch status of the server is displayed in the Servers & Services section. A check mark next to the server/service indicates that this server/service will start/stop when the Servers button is pressed.  The Apache web server (default web server) uses port 8888 by default. This port must be specified when calling the local web page in the browser, e.g.: http://localhost:8888

Your default host for MAMP PRO is `localhost`. The files for localhost are initially located in the `C:\MAMP\htdocs` folder. Press the Open button located to the right of the Host-Name text box to open up the localhost in your default web browser.

![MAMP](/en/MAMP-PRO-Windows/First-Steps/OpenLocalHost.png)

<div class="alert" role="alert">
Note: Although the default localhost document root is located in `C:\MAMP\htdocs`, it is best to keep it's document root, and the document root of additional hosts out of the `C:\MAMP` folder. A better directory structure for your host document root folders would be `~\sites\localhost`, `~\sites\site1`, `~\sites\site2`, etc ... .
</div>

---

### Add Additional Hosts

To add an additional host press the '+' button at the bottom left corner of the Hosts table. You will then be asked to select a document root folder and optionally a database. See the [Hosts](../Settings/Hosts/General) section for more information on what a host is and how to create additional hosts.

---

### Main GUI Elements

*  **MAMP PRO**  
   Open the  [https://mamp.info](https://www.mamp.info){:target="_blank"} web page.
*  **Editor**  
   Open the MAMP PRO Editor. Additional information about the MAMP PRO Editor can be found in the [Editor](../Editor/)
   section.
*  **WebStart**  
   Open the MAMP PRO start page of your local web server.
   Additional information about the MAMP PRO start page is in the [Webstart](../WebStart) section.
*  **Start/Stop**  
   Starts the current GroupStart services of MAMP PRO. Stops all services if any GroupStart services are already running. 
   
---

### Meaning of Icons


![MAMP](/en/MAMP-PRO-Mac/First-Steps/info.png) Provide more information, including phpInfo().

![MAMP](/en/MAMP-PRO-Mac/First-Steps/RedArrow.png) Indicates that information is missing.

![MAMP](/en/MAMP-PRO-Mac/First-Steps/Plus.png) Add a new PHP version.
