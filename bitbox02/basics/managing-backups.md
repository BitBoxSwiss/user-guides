---
layout: default
title: Managing backups
nav_order: 5
has_children: false
parent: Basic features
grand_parent: BitBox02
---

# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---
## What is a wallet backup & what are recovery words?
Modern cryptocurrency wallets calculate all keys from a single secret, the master seed. From that, an unlimited number of currencies, accounts and addresses can be derived. This means that you only need to back up the master seed **once**, and the whole wallet, **including all future transactions**, can be recovered from this backup.

This single secret is a very long random number. To make it easier to write it down, the secret number is encoded into 24 English recovery words:

- Words from a fixed and well-known list of 2048 words are used.
- The first four characters already identify each word uniquely, but writing the whole word adds better readability.
- An integrated consistency check during set-up of the wallet helps to detect mistakes.

When you set up your BitBox02 wallet, it automatically saved a wallet backup to a microSD card. Please store that microSD card in a secure location.

## Where should I store my wallet backup?
It is crucial, that your wallet backup(s) are stored in a secure location. If anyone get's access to your wallet backup, they can restore your wallet and steal your funds. Depending on the value you're securing, choose an appropriate location, for example a locked drawer, a safe at home or a safety deposit box.

Be aware that the physical security of your backup is more important than that of your hardware wallet. A hardware wallet protects your cryptocurrencies even in the hand of a thief, but these recovery words allow direct access to your funds.

[Optionally you can use a passphrase, which gives additional protection for your wallet backups.]({% link bitbox02/advanced/passphrase.md %})

## MicroSD card wallet backup
Please make sure you have the microSD card that contains your backup inserted into your BitBox02.

### How should I handle my wallet backup?
Your wallet backup contains your private keys and anyone who knows these words has full control over all your funds secured in the corresponding wallet.
To make sure that your recovery words are safe, follow this advice:
- Store your wallet backup in a secure location.
- Do not insert your microSD card backup into a computer, phone, printer or any device other than a BitBox02.

### Listing the backup files
In order to check which backup files are on your microSD card, click "Manage Backups"
![alt text]({% link assets/images/BitBox02_backups/backups1.png %})
You will then see a list of all backup files found on the currently inserted microSD card.

Normally that is just one file:
![alt text]({% link assets/images/BitBox02_backups/backups2.png %})
### Verifying a backup
In order to verify, that one of the backup files on the currently inserted microSD card is a backup of the wallet you are currently using on your BitBox02 (and not a backup of some other, older wallet which you might not be using anymore) click "Check Backup".

You should then see a pop-up like this:

![alt text]({% link assets/images/BitBox02_backups/backups3.png %})

That pop-up tells you that there is a backup for the currently used wallet, i.e. in this case there is a backup for the wallet called "Tutorial-2" which is the wallet I'm currently using.

You are then asked to confirm that the ID shown in the BitBoxApp matches the ID shown on your BitBox02.
If that is the case please confirm on your BitBox02 and then click "OK" in the BitBoxApp.

### Creating a new backup
If your backup was destroyed or you would just like to create another backup to store in a different location you can easily do that. All you need is a fresh microSD card which the new backup will be stored on.

{% include shared/microSD.md %}

### Plug in the new microSD card and click "Manage Backups"
{: .no_toc }
![alt text]({% link assets/images/BitBox02_backups/backups1.png %})

### Click "Create Backup"
{: .no_toc }
![alt text]({% link assets/images/BitBox02_backups/backups4.png %})

### Follow instructions on your BitBox02
{: .no_toc }
Next you should see a pop-up telling you to follow the instructions on your BitBox02 screen.

![alt text]({% link assets/images/BitBox02_backups/backups5.png %})

<!--On your BitBox02 you will first need to confirm that you understand that **by default backup files are not password protected, i.e. if someone finds your backup they can steal your coins**.-->

Then you will be asked to input your device password to confirm the backup creation.

Once confirmed, you backup will be created and saved to the microSD card.

If you would like to manually check that there now is a backup file on the microSD card, please click "Back" once, then "Manage Backups" again and then [verify your backup.]({% link bitbox02/basics/managing-backups.md %}#verifying-a-backup)

## Optional backup via recovery words
> **Note:** It is not necessary to write down your recovery words as you have already created a wallet backup onto a microSD card when you initialised your BitBox02. This is an advanced feature.

### How should I handle my recovery words?
Before starting to write down your recovery words, be aware that this is a backup of your private keys and anyone who knows these words has full control over all your funds secured in the corresponding wallet.
To make sure that your recovery words are safe, follow this advice:
- Use a private environment, don't let anyone else see your recovery words and don't spell them out loud.
- No digital picture, especially not with your smartphone.
- No online backup, like in a key manager or a cloud service.
- No photocopy, as all modern copy machines are digital and store copies.
- Never enter your recovery words on a computer.

### Show recovery words
In "Device settings" click "Show recovery words".
![alt text]({% link assets/images/BitBox02_mnemonic/bip39_1.png %})

You will then see the following warning, which you need to confirm in order to display your recovery words on your BitBox02.
![alt text]({% link assets/images/BitBox02_mnemonic/bip39_2.png %})

Next you will be asked to confirm that you want to display your recovery words by typing in your device password on the BitBox02.

### Write down your recovery words
Once you have typed in your correct device password, your recovery words will be displayed on your BitBox02. You can use the touch buttons to navigate through the words.

Please write down each word carefully.

### Confirm your recovery words
Next you will be asked to confirm your recovery words by selecting the correct word for each position from a choice of five words.
