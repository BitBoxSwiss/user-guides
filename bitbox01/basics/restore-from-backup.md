---
layout: default
title: Restore from backup
seo_title: BitBox01 - Restore from backup
nav_order: 6
parent: Basic features
grand_parent: BitBox01
description: Find out how to restore your BitBox01 wallet from your microSD card backup.
---

# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---

In order to restore your wallet from your backup you need:
- A BitBox01
- Your microSD card which contains your wallet backup file
- Your backup recovery password

## Install the latest BitBoxApp
You should always use the latest BitBoxApp.

[Download](https://shiftcrypto.ch/download/){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }

### BitBox01 not detected
If your BitBox01 has not been updated in a long time the latest BitBoxApp will not detect it.
In that case you need to install version 3.0.0 of the old DigitalBitBoxApp and upgrade your BitBox01 firmware with that app. Once done, quit the DigitalBitBoxApp and launch the latest BitBoxApp again. The latest BitBoxApp will then detect your BitBox01.

[Download old DigitalBitBoxApp](https://github.com/digitalbitbox/dbb-app/releases/tag/v3.0.0){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }


## Plug in the microSD card with your backup and plug in the BitBox01
In order to be able to restore from a backup file, the microSD card with the backup on it needs to be inserted into the BitBox01. Once done, plug in your BitBox01.


## Choose that you want to restore from a backup file
Please select that you want to restore from a backup file on your microSD card by clicking "Restore a wallet from a backup".
![alt text]({% link assets/images/BitBox01_setup/bb01_setup1.png %})

## Start the restoring process
The BitBoxApp will now remind you that your microSD card with your backup file needs to be inserted into the BitBox01 and that you will need recovery password.

Click "Continue"

![alt text]({% link assets/images/BitBox01_restore/bb01_restore1.png %})

## Set device password
Please choose a device password. That password can be changed later.

![alt text]({% link assets/images/BitBox01_restore/bb01_restore2.png %})
![alt text]({% link assets/images/BitBox01_restore/bb01_restore3.png %})

## Restore your wallet
Next you will choose the wallet backup file you want to restore from and input the corresponding recovery password.
Click "Continue"
![alt text]({% link assets/images/BitBox01_restore/bb01_restore4.png %})

Select the wallet backup file and click "Restore"
![alt text]({% link assets/images/BitBox01_restore/bb01_restore5.png %})

Next input the recovery password for that wallet.

**Attention:** There will be no error if you input a different backup recovery password than the one you used when you created your wallet. The BitBox01 does not store information about your recovery password and therefore can't "check" if it is the same one you used before or not.
If you cannot find your funds after you restored you have most likely inputed a different recovery password. In that case, please restore from your backup again and make sure that you input the same recovery password you used when you created your wallet.

> If you created your wallet before Aug 2018, then your backup recovery password is identical to your normal device password.

Check the box and click "Restore".

![alt text]({% link assets/images/BitBox01_restore/bb01_restore7.png %})

You have successfully restored your wallet.

>Please make sure you store your backup microSD card in a secure location and that you don't lose your recovery password.
**Reminder:** Only the backup microSD + recovery password allows you to restore your wallet. **One of the two is not enough.**

![alt text]({% link assets/images/BitBox01_restore/bb01_restore8.png %})
