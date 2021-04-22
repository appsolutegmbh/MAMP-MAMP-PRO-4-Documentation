---
title: MAMP PRO (Windows) Documentation > New MAMP PRO Installation
description: 
layout: default-2
product: MAMP PRO Windows
language: en
lastedit: 2021-04-16
---

## New MAMP PRO Installation

1. Download MAMP PRO from [www.mamp.info](https://www.mamp.info/downloads){:target="_blank"}.
2. Double click on the MAMP_MAMP_PRO_4.X.X.exe file in your Downloads folder.
3. The Windows Installer will guide you through the installation process.

---

### Install Location

MAMP and MAMP PRO can be installed on any standard Windows drive such as C:, D:, E:, etc. For simplicity, we recommend installing in the default directory (C:\MAMP). We strongly advise against installing MAMP and MAMP PRO in a system folder because the MAMP servers (Apache, MySQL, Nginx) require write permissions for the folders "log", "configuration", "htdocs" and "databases". These cannot be granted by the Windows security concept if MAMP and MAMP PRO have been installed in the Program Files, Windows, User directory or another system folder. Changing the settings of User Account Control (UAC), Windows Defender and work privileges is not a recommended way of maintaining the security of the system.

By default, MAMP/MAMP PRO will be installed in your "C:\MAMP" and "C:\MAMP PRO" folders.

![MAMP](/en/MAMP-PRO-Windows/Installation/New-Install/InstallLocation.png)

### Apple Bonjour

By default, Apple Bonjour will be installed when you install MAMP PRO. You will not have access to your hosts from the MAMP Viewer if you choose not to install Apple Bonjour.

![MAMP](/en/MAMP-PRO-Windows/Installation/New-Install/InstallBonjour.png)

### Windows Defender

You may receive a warning from Windows Defender when installing MAMP PRO. This is standard firewall behavior for Windows applications started as servers. You may 'Allow access' for private networks and public networks depending on your implementation needs. You can later change your Windows firewall permissions as necessary.

![MAMP](/en/MAMP-PRO-Windows/Installation/New-Install/defender.png)