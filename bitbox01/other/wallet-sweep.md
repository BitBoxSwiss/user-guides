---
layout: default
title: Sweep guide
seo_title: BitBox01 - How to sweep my wallet?
nav_order: 5
has_children: false
parent: Other guides
grand_parent: BitBox01
description: This guide explains how to sweep the coins in your BitBox01 wallet to another wallet. 
---
# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

Please make sure that you have the latest firmware. To download click [here](https://shiftcrypto.ch/start/).
This guide demonstrates how to sweep all funds from an old BitBox01 (aka. Digital BitBox) wallet onto a newly created wallet from both standard and (optionally) hidden wallets. The basic procedure is:
1. Verify you the backup of your current wallet
2. Reset your BitBox01
3. Create new wallet
4. Save receive addresses
5. Restore old wallet
6. Send coins to the saved receive addresses
7. Use new wallet



## Verify that you have a valid backup and recovery password
Please check [this guide]({% link bitbox01/basics/managing-backups.md %}#bitbox01-managing-backups) to verify that you have valid wallet backup and recovery password for the wallet you want to send your coins out of.

If that is the case you can proceed.
If you can't verify that your backup and and recovery password contact support by clicking on the "Contact Us" button on the lower right of this page.

## Create new wallet
>**Attention:** If you did not verify that you have a valid backup and recovery password you might forever lose your coins. Only reset your device if you verified that you indeed have a valid backup and recovery password. To verify your backup follow [this guide]({%link bitbox01/basics/managing-backups.md %}#verifying-a-backup)


1. To reset your BitBox01 follow [this guide]({% link bitbox01/advanced/reset.md %})
2. Now create the new wallet to which you want to send your coins. Follow [this guide]({% link bitbox01/setup.md %}) to do so.


### Verify and save receive addresses
{: .no_toc }
Your BitBox01 should still be plugged in and unlocked.
1. [Verify and copy a receive address from your BitBox01]({% link bitbox01/basics/receive.md %}) for each coin you want to sweep (i.e. Bitcoin, Litecoin) and paste it into a text file. Make sure you carefully check that it has been copied correctly.
>The receive address is where your will send your funds to. Note that for Bitcoin, you may have had different style bitcoin addresses in your old wallet that each held funds. These funds can all be sent to the same (default) style receive address you just copied and stored.

### Optional: Hidden wallet
Your BitBox01 should still be plugged in and unlocked in the newly created wallet.
- Go to "Manage Device", click "Create Hidden Wallet" and follow the on-screen instructions.

In order to get a receive address for the Hidden Wallet, unplug and reinsert the BitBox and log in using the hidden wallet password. Again copy and store the receive address in a text document as described in the previous step.

Please make sure you properly separate the receive addresses for the normal wallet and the hidden wallet addresses in order to not mix them up.

If you are using MyEtherWallet for Ethereum or other coins they support: Log in to the MyEtherWallet website, follow their instructions for obtaining a receive address. Copy and save this address.



## Restore your old wallet
In order to access your old wallet again (which still holds your coins) you need to reset the BitBox01 again and then reload the old wallet from the backup.
1. To reset your BitBox01 follow [this guide]({% link bitbox01/advanced/reset.md %})
2. Please follow [this guide]({% link bitbox01/basics/restore-from-backup.md %}) to restore your old wallet.

## Send coins from old to new wallet
Your BitBox01 should be plugged in and unlocked.

1. Select a currency (e.g. Bitcoin) and click "Send".
2. Paste the respective address from the new wallet that you stored in a text file into the appropriate field, and select the "Send all" checkbox to send all funds.
3. Before you hit send, make sure you have pasted the address into the send field accurately by visually comparing it to what you have in, for example, the text document.
4. Confirm and send your transaction.
5. Reapeat steps 1-3 for all currency and types (e.g. Bitcoin has multiple address types, you can select all of them in the BitBoxApp settings) that you want to sweep form your old wallet to your new wallet.

## If you have funds stored in a hidden wallet:
Funds in a hidden wallet may also be sent to a new standard wallet. However, note that doing so affects privacy: this would create a connection between the previously separately stored funds that could be revealed by someone analysing the public blockchain. Therefore, you may wish to send funds in a hidden wallet to a new hidden wallet.

How to access a hidden wallet depends on if you are using a legacy version of the hidden wallet or the current version of the hidden wallet. You are using a legacy hidden wallet if it was created using desktop app versions before version 3.0.0.

If using a legacy version, you can most likely access the funds by simply unplugging and reinserting the device then logging in using the hidden wallet password.

If this does not work, log in the old (standard) wallet and try activating legacy mode: Go to Manage Device, expand the Guide section on the right and then expand the section How do I access the legacy hidden wallet. Here you can enable the legacy hidden wallet mode. Next, unplug and re-insert the device, then login using the hidden wallet password.

If you are using a current version of the hidden wallet, it can be re-enabled by logging into the old (standard) wallet, then go to Manage Device, choose Create Hidden Wallet, and follow the on-screen instructions. Be sure to enter the old recovery password that was used for the hidden wallet. Unplug and reinsert the BitBox and then enter in your legacy hidden wallet password to access the funds.

Once in the hidden wallet, simply sweep your funds following the same instructions above for the standard wallet. Send the funds to a receive address from a new hidden wallet if you wish to preserve privacy.

If you are using MyEtherWallet for Ethereum or other coins they support: Log in to the MyEtherWallet website, follow their instructions for sending funds, and send to the new receive address stored in the previous step.

## Restore the new wallet
After you have moved all your funds to your new wallet, return to step 2, but this time use the new wallet recovery password instead of the old one. There you should see your funds.
