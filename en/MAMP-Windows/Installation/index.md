---
title: MAMP PRO (Windows) Documentation > MAMP (Windows) Installation
description:
layout: default-2
product: MAMP Windows
language: en
lastedit: 2021-04-20
---

## Installation

### Installation Requirements

To use MAMP, your system must meet the following requirements:

- Microsoft Windows 10+ (32-bit or 64-bit). MAMP 4 will work Windows Server OS (although not officially supported).
- 1GB RAM
- .NET Framework 4.0

---

### New Installation

1. Download MAMP PRO from [www.mamp.info](https://www.mamp.info){:target="_blank"}.
2. Double click on the file "setup_MAMP_MAMP_PRO_4.x.exe" in your Downloads folder.
3. The Windows Installer will guide you through the installation process.

MAMP and MAMP PRO can be installed on any standard Windows drive such as C:, D:, E:, etc. For simplicity, we recommend installing in the default directory (C:\MAMP). We strongly advise against installing MAMP and MAMP PRO in a system folder because the MAMP servers (Apache, MySQL, Nginx) require write permissions for the folders "log", "configuration", "htdocs" and "databases". These cannot be granted by the Windows security concept if MAMP and MAMP PRO have been installed in the Program Files, Windows, User directory or another system folder. Changing the settings of User Account Control (UAC), Windows Defender and work privileges is not a recommended way of maintaining the security of the system.

When installing MAMP, both a "C:\MAMP PRO" and "C:\MAMP" folder will be installed. You can ignore the "C:\MAMP PRO" folder if you choose not use MAMP PRO.

---

### Upgrade From MAMP 3

You should backup your database data before upgrading from MAMP 3 to MAMP 4. Your database data is located in "C:\MAMP\db".

1. Download MAMP PRO from [www.mamp.info](https://www.mamp.info){:target="_blank"}.
2. Double click on the file "setup_MAMP_MAMP_PRO_4.0.exe" in your Downloads folder.
3. The Windows Installer will guide you through the installation process.

### Upgrading MySQL Data

MAMP 4 uses MySQL 5.6. You must first install MAMP 3.3 or greater in order to install MAMP 4. 

---

### Uninstall

Use Add/Remove programs from Control Panel to uninstall MAMP. The Windows Uninstaller will also uninstall MAMP PRO.