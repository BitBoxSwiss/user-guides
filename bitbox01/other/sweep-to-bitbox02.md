---
layout: default
title: Sweep funds from BitBox01 to BitBox02
seo_title: How to transfer my coins from a BitBox01 to BitBox02?
nav_order: 4
has_children: false
parent: Other guides
grand_parent: BitBox01
description: This guide explains how to transfer the coins stored on your BitBox01 to a BitBox02 hardware wallet.
---
# {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---
This guide demonstrates how to sweep all funds from a BitBox01 (aka. Digital BitBox) onto a newly created wallet on a BitBox02 from both standard and (optionally) hidden wallets. The basic procedure is:
1. Setup your BitBox02
2. Send coins from BitBox01 to BitBox02
3. Use BitBox02

* Optional: Ethereum sweep (todo)


## Setup your BitBox02
If you have not yet set up your BitBox02, please follow
[this guide]({% link bitbox02/setup.md %}) to do so.


### Did you use the hidden wallet option on the BitBox01 (aka. Digital BitBox) and you want to continue using it?

**If no:** [Click here to continue](#send-coins-from-bitbox01-to-bitbox02-no-hidden-wallet)

**If yes:** [Click here to continue](#send-coins-from-bitbox01-to-bitbox02-with-hidden-wallet)

## Send coins from BitBox01 to BitBox02 (no hidden wallet)
Your BitBox02 should still be plugged in and unlocked.
1. [Verify and copy a receive address from your BitBox02]({% link bitbox02/basics/receive.md %}) for each coin you want to sweep (i.e. Bitcoin, Litecoin) and paste it into a text file. Make sure you carefully check that it has been copied correctly.
>The receive address is where your will send your funds to from the BitBox01 to the BitBox02. Note that for Bitcoin, you may have had different style bitcoin addresses in your old wallet that each held funds. These funds can all be sent to the same (default) style receive address you just copied and stored.

2. Once you have the receive addresses copied into a text file and double checked you can unplug your BitBox02.
3. Then plug in your BitBox01 and unlock it with your BitBox01 device password as usual.
4. Select a currency (e.g. Bitcoin) and click "Send".
5. Paste the respective receive address from your text file into the address field, choose a low test amount (e.g. 2 USD) and select a low fee. Make sure you pasted the correct address that matches (i.e. Bitcoin address for Bitcoin transaction).
6. Confirm and send your transaction.
7. Repeat steps 4-6 for all currency and types (e.g. Bitcoin has multiple address types, you can select all of them in the BitBoxApp settings) that you want to sweep form your BitBox01 to BitBox02.
8. Remember how many test transactions you made.
9. Unplug your BitBox01, plug in your BitBox02, unlock it with your BitBox02 device password.
10. Check that all test transactions arrived on your BitBox02 ([you might need to enable more coins/types in the BitBoxApp settings]({%link bitboxapp/settings.md %}#troubleshooting-my-coins-are-gone-after-bitboxapp-update)).

**If that is the case:**

Repeat steps 3-10 with real amounts. You can split it up into multiple transactions if you feel uncomfortable sending all in one transaction. Please confirm that it was received on the BitBox02 after each transaction.

If you can't see all your test transactions after a few minutes:

{% include contact.html url=page.url %}


## Send coins from BitBox01 to BitBox02 (with hidden wallet)
A) If you didn't use the hidden wallet feature on the BitBox01: [Click here](#send-coins-from-bitbox01-to-bitbox02-no-hidden-wallet)

B) If you used the hidden-wallet feature but you don't want to continue using it on your BitBox02: [Click here](#send-coins-from-bitbox01-to-bitbox02-no-hidden-wallet) and repeat it once to sweep the standard wallet from your BitBox01 and then again to sweep the hidden-wallet from your BitBox01.

C) If you used the hidden-wallet feature and you want to continue using it on your BitBox02 continue reading.




### Prerequisites
* Your BitBox02 should still be plugged in and unlocked.

* "Mnemonic Passphrase" should be enabled on your BitBox02, see [here]({% link bitbox02/advanced/passphrase.md %})

Now we need to do two wallet sweeps.
* Standard wallet sweep
* Hidden wallet sweep

### Standard wallet sweep
1. [Verify and copy a receive address from your BitBox02]({% link bitbox02/basics/receive.md %}) for each coin you want to sweep (i.e. Bitcoin, Litecoin) and paste it into a text file, note down that this address is from the standard wallet. Make sure you carefully check that it has been copied correctly.
> The receive address is where your will send your funds to from the BitBox01 to the BitBox02. Note that for Bitcoin, you may have had different style bitcoin addresses in your old wallet that each held funds. These funds can all be sent to the same (default) style receive address you just copied and stored.

2. Once you have the receive addresses copied into a text file and double checked that it is correct you can unplug your BitBox02.
3. Then plug in your BitBox01 and unlock it with your BitBox01 device password as usual.
4. Select a currency (e.g. Bitcoin) and click "Send".
5. Paste the respective receive address from your text file into the address field, choose a low test amount (e.g. 2 USD) and select a low fee. Make sure you pasted the correct address that matches (i.e. Bitcoin address for Bitcoin transaction)
6. Confirm and send your transaction.
7. Repeat steps 4-6 for all currency and types (e.g. Bitcoin has multiple address types, you can select all of them in the BitBoxApp settings) that you want to sweep form your BitBox01 to BitBox02.
8. Remember how many test transactions you made.
9. Unplug your BitBox01, plug in your BitBox02, unlock it with your BitBox02 device password.
10. Check that all test transactions arrived on your BitBox02 ([you might need to enable more coins/types in the BitBoxApp settings]({%link bitboxapp/settings.md %}#troubleshooting-my-coins-are-gone-after-bitboxapp-update)).

**If that is the case:**

>Repeat steps 3-10 with real amounts. You can split it up into multiple transactions if you feel uncomfortable sending all in one transaction. Please confirm that it was received on the BitBox02 after each transaction.

If you can't see all your test transactions after a few minutes:

{% include contact.html url=page.url %}


### Hidden-wallet sweep
>**DANGER:** If you forget/lose this passphrase you will forever lose access to the coins stored in that hidden wallet. Proceed with caution.

1. Generate a new passphrase for the hidden wallet to use on your BitBox02 (or re-use the old "hidden-wallet" password if you are sure it is secure) and make sure to back this passphrase up (**important!!**)
2. Unplug your BitBox02, plug it in again, type in your BitBox02 device password.
3. Then type in your passphrase for your hidden wallet which you generated in step 1.
>**Attention:** If you forget/lose this passphrase you will lose access to the coins in this wallet. Make sure to backup the passphrase properly.


4. [Verify and copy a receive address from your BitBox02]({% link bitbox02/basics/receive.md %})  for each coin you want to sweep (i.e. Bitcoin, Litecoin) and paste it into a text file, note down that this address is from the hidden wallet. Make sure you carefully check that it has been copied correctly.
>The receive address is where your will send your funds to from the BitBox01 to the BitBox02. Note that for Bitcoin, you may have had different style bitcoin addresses in your old wallet that each held funds. These funds can all be sent to the same (default) style receive address you just copied and stored.

5. Once you have the receive addresses copied into a text file and double checked you can unplug your BitBox02.
6. Then plug in your BitBox01 and unlock it with your BitBox01 device password as usual.
7. Select a currency (e.g. Bitcoin) and click "Send".
8. Paste the respective receive address from your text file into the address field, choose a low test amount (e.g. 2 USD) and select a low fee. Make sure you pasted the correct address that matches (i.e. Bitcoin address for Bitcoin transaction).
9. Confirm and send your transaction.
10. Repeat steps 6-9 for all currency and types (e.g. Bitcoin has multiple address types, you can select all of them in the BitBoxApp settings) that you want to sweep form your BitBox01 to BitBox02.
11. Remember how many test transactions you made.
12. Unplug your BitBox01, plug in your BitBox02, unlock it with your BitBox02 device password.
13. Check that all test transactions arrived on your BitBox02 ([you might need to enable more coins/types in the BitBoxApp settings]({%link bitboxapp/settings.md %}#troubleshooting-my-coins-are-gone-after-bitboxapp-update)).

**If that is the case:**

>Repeat steps 6-13 with real amounts. You can split it up into multiple transactions if you feel uncomfortable sending all in one transaction. Please confirm that it was received on the BitBox02 after each transaction.

If you can't see all your test transactions after a few minutes:

{% include contact.html url=page.url %}


## Use your BitBox02
After you have moved all your funds to your new BitBox02 you are good to go.
Have fun and always stay safe.

Kind regards, Shift Crypto Team.
