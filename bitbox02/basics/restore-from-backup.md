---
layout: default
title: Restore from backup
seo_title: BitBox02 - How to restore from a microSD card backup?
nav_order: 6
parent: Basic features
grand_parent: BitBox02
description: Find out how to restore your wallet from your microSD card.
---

# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---

In order to restore from a backup, your BitBox02 needs to be reset.

## Plug in the microSD card containing your backup and plug in the BitBox02
In order to be able to restore from a backup, the microSD card containing the backup needs to be inserted. Once done, plug in your BitBox02 with the BitBoxApp open.

As your device is reset, you will first need to pair it again.

Please compare the code on your BitBox02 and in the BitBoxApp and confirm on your BitBox02 if they match. Then click "Confirm & Continue" in the BitBoxApp.
![alt text]({% link assets/images/BitBox02_restore/restore1.png %})

## Choose that you want to restore from a backup file
Please select that you want to restore from a backup file on your microSD card by clicking "Restore from microSD card".
![alt text]({% link assets/images/BitBox02_restore/restore2.png %})

## Choose backup file
The BitBoxApp will now remind you that your microSD card with your backup needs to be inserted if not already done.

Next you will see a list of all backup files that were found on your microSD card.

In most cases that would just be one file.

Select the wallet you want to restore and click "Restore".


![alt text]({% link assets/images/BitBox02_restore/restore3.png %})


## Choose device password
Next you will need to input a device password on your BitBox02. You will need this password every time you want to use your BitBox02.

Please input and confirm the device password on your BitBox02 and afterwards confirm today's date.
![alt text]({% link assets/images/BitBox02_restore/restore4.png %})

## Done! Start using your BitBox02
You have successfully restored your wallet and can continue using your BitBox02 as usual.

**Please make sure you store your backup microSD card in a secure location**. Anyone that finds it can steal your coins unless you use an additional [passphrase]({% link bitbox02/advanced/passphrase.md %})
![alt text]({% link assets/images/BitBox02_restore/restore5.png %})
