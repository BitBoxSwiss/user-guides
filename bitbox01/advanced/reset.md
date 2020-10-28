---
layout: default
title: Reset device
seo_title: BitBox01 - Reset device
nav_order: 2
parent: Advanced features
grand_parent: BitBox01
description: Find out how to reset your BitBox02 hardware wallet.
---
# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---

## Make sure you have your backup
**Caution:** Resetting your device deletes all data, including your seed (i.e. your wallet), from the device. It is essential that you have a working backup of your wallet before you reset your BitBox01. If that is not the case you will most likely **forever lose your coins!!!**
To check if you have a valid backup and recovery password follow [this guide]({% link bitbox01/basics/managing-backups.md %}#verifying-a-backup)

## Resetting your BitBox01
### Reset without device unlock
If you want to reset your BitBox01 without the BitBoxApp, just type in an incorrect device password 10 times. Then your BitBox01 will reset to factory reset.

### Reset via the BitBoxApp
Go to "Device Settings" and select "Reset Device."
![alt text]({% link assets/images/BitBox02_reset/reset1.png %})

Then type in your device password in order to confirm that you want to reset the BitBox01, tick the box to confirm that you have a valid backup and recovery password (if you are not sure, please verify by following [this guide]({% link bitbox01/basics/managing-backups.md %}#verifying-a-backup)) and click "Reset Device".
![alt text]({% link assets/images/BitBox01_random/bb01_reset.png %})
