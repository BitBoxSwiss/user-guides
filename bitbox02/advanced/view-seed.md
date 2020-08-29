---
layout: default
title: Display recovery words
nav_order: 2
parent: Advanced features
grand_parent: BitBox02

---
# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---
If you want to make a backup to a microSD card, [follow this guide]({% link bitbox02/basics/managing-backups.md %}#creating-a-new-backup )

Continue reading if you want to display your wallet recovery words (also called "mnemonic seed") on your BitBox02 in order to write it on paper or punch it into metal.

## What is a wallet backup & what are recovery words?
Modern cryptocurrency wallets calculate all keys from a single secret, the master seed. From that, an unlimited number of currencies, accounts and addresses can be derived. This means that you only need to back up the master seed **once**, and the whole wallet, **including all future transactions**, can be recovered from this backup.

> **Note:** It is not necessary to write down your recovery words as you have already created a wallet backup onto a microSD card when you initialised your BitBox02. This is an advanced feature.

This single secret is a very long random number. To make it easier to write it down, the secret number is encoded into 24 English recovery words:

- Words from a fixed and well-known list of 2048 words are used.
- The first four characters already identify each word uniquely, but writing the whole word adds better readability.
- An integrated consistency check during set-up of the wallet helps to detect mistakes.

## Where should I store my backup?
Already think about where to safely store the backup card before writing down your recovery words. Depending on the value you're securing, choose an appropriate location, for example a locked drawer, a safe at home or a safety deposit box.

Be aware that the physical security of your recovery words is more important than that of your hardware wallet. A hardware wallet protects your cryptocurrencies even in the hand of a thief, but these recovery words allow direct access to your funds.

## How should I handle my recovery words?
Before starting to write down your recovery words, be aware that this is a backup of your private keys and anyone who knows these words has full control over all your funds secured in the corresponding wallet.
To make sure that your recovery words are safe, follow this advice:
- Use a private environment, don't let anyone else see your recovery words and don't spell them out loud.
- No digital picture, especially not with your smartphone.
- No online backup, like in a key manager or a cloud service.
- No photocopy, as all modern copy machines are digital and store copies.
- Never enter your recovery words on a computer.


## Show recovery words
In "Device settings" click "Show recovery words".
![alt text]({% link assets/images/BitBox02_mnemonic/bip39_1.png %})

You will then see the following warning, which you need to confirm in order to display your recovery words on your BitBox02.
![alt text]({% link assets/images/BitBox02_mnemonic/bip39_2.png %})

Next you will be asked to confirm that you want to display your recovery words by typing in your device password on the BitBox02.

## Write down your recovery words
Once you have typed in your correct device password, your recovery words will be displayed on your BitBox02. You can use the touch buttons to navigate through the words.

Please write down each word carefully.

## Confirm your recovery words
Next you will be asked to confirm your recovery words by selecting the correct word for each position from a choice of five words.
