---
layout: default
title: Import wallet
seo_title: BitBox02 - How to import a wallet backup onto a BitBox02?
nav_order: 6
parent: Basic features
grand_parent: BitBox02
description: Find out how to import a wallet onto the BitBox02.
---

# {{page.grand_parent}}: {{page.title}}

Find the right section for your circumstances:
- Your wallet was created on a BitBox02:
  - [You want to import your wallet from your microSD card backup]({% link bitbox02/basics/import-wallet.md %}#import-wallet-from-microsd-card-backup)
  - [You want to import your wallet from your 24 recovery words]({% link bitbox02/basics/import-wallet.md %}#import-wallet-from-recovery-words)
- Your wallet was not created on a BitBox02:
  - [You want to import your wallet from your 24 recovery words created by a different wallet]({% link bitbox02/basics/import-wallet.md %}#import-wallet-from-recovery-words)
- You lost your BitBox02 and want to export your BitBox02 wallet into a different hardware wallet:
  - [You want to export your BitBox02 wallet into a different wallet]({% link bitbox02/basics/export-wallet.md %}#export-bitbox02-wallet-into-third-party-wallet)

## Import wallet from microSD card backup
### Plug in the microSD card containing your backup and plug in the BitBox02
In order to be able to restore from a backup, the microSD card containing the backup needs to be inserted. Once done, plug in your BitBox02 with the BitBoxApp open.

As your device is reset, you will first need to pair it again.

Please compare the code on your BitBox02 and in the BitBoxApp and confirm on your BitBox02 if they match. Then click "Confirm & Continue" in the BitBoxApp.
![alt text]({% link assets/images/BitBox02_restore/restore1.png %})

### Choose that you want to restore from a backup file
Please select that you want to restore from a backup file on your microSD card by clicking "Restore from microSD card".
![alt text]({% link assets/images/BitBox02_restore/restore2.png %})

### Choose backup file
The BitBoxApp will now remind you that your microSD card with your backup needs to be inserted if not already done.

Next you will see a list of all backup files that were found on your microSD card.

In most cases that would just be one file.

Select the wallet you want to restore and click "Restore".

![alt text]({% link assets/images/BitBox02_restore/restore3.png %})

### Choose device password
Next you will need to input a device password on your BitBox02. You will need this password every time you want to use your BitBox02.

Please input and confirm the device password on your BitBox02 and afterwards confirm today's date.
![alt text]({% link assets/images/BitBox02_restore/restore4.png %})

### Done! Start using your BitBox02
You have successfully restored your wallet and can continue using your BitBox02 as usual.

**Please make sure you store your wallet backup in a secure location**. Anyone that finds it can steal your coins unless you use an additional [passphrase]({% link bitbox02/advanced/passphrase.md %})
![alt text]({% link assets/images/BitBox02_restore/restore5.png %})

## Import wallet from recovery words
>**Attention**: The BitBox02 only supports Segwit (starting with 3...) and Native-Segwit (starting with bc1....) accounts. If you import a seed phrase that you used with the Legacy address format (starting with 1...) you won't see these coins in the BitBoxApp. We recommend you to move these coins to a Segwit or Native-Segwit account.

### Choose that you want to restore from recovery words
Please select that you want to restore your recovery words by clicking "Restore from recovery words" and follow the instructions on the display of your BitBox02.

![alt text]({% link assets/images/BitBox02_restore/restore2.png %})

### Select how long your mnemonic seed phrase is
On your BitBox02, select how long your mnemonic seed phrase is. (12, 18 or 24 recovery words)

### Enter each recovery word on BitBox02
Now enter each recovery word on your BitBox02. The BitBox02 will auto-complete your input once it is clear which word you are trying to enter. After each word, confirm by tapping the tick in the upper right corner.

### Verify recovery words on BitBox02
Once you have entered all recovery words, the BitBox02 will display them again and ask you to confirm that the input is correct.

### Choose device password
Next you will need to input a device password on your BitBox02. You will need this password every time you want to use your BitBox02.

Please input and confirm the device password on your BitBox02 and afterwards confirm today's date.
![alt text]({% link assets/images/BitBox02_restore/restore4.png %})

### Done! Start using your BitBox02
You have successfully restored your wallet and can continue using your BitBox02 as usual.

**Please make sure you store your wallet backup in a secure location**. Anyone that finds it can steal your coins unless you use an additional [passphrase]({% link bitbox02/advanced/passphrase.md %})
![alt text]({% link assets/images/BitBox02_restore/restore5.png %})
