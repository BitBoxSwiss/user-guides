---
layout: default
title: Blockchain Forks
nav_order: 1
has_children: false
parent: Other

---

# {{page.parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## General information on Bitcoin chain forks

### Background
In the future, the Bitcoin blockchain may fork or split. This occurs when a portion of Bitcoin nodes run software that is not fully compatible with other nodes. Chain forks occur in order to update the Bitcoin protocol. A chain fork could be thought of as a vote about how best to improve Bitcoin. However, a chain fork may result in unreliable transactions for an unknown length of time. Furthermore, if different groups have different ideas about how to best improve Bitcoin, it may be hard to predict how the community as a whole will value (i.e. price) coins in each side of the chain fork.

The good news is that coins held in a BitBox are completely safe.
The BitBox itself and any coins secured by the device do not depend on the type of nodes active. When a chain fork occurs, you automatically now own coins on both sides of the fork, or, in other words, coins on each chain. All coins held in the device CANNOT be lost (unless you lose your password). All coins are safe no matter what happens in a future chain fork.

However, risks exist when sending and possibly receiving coins.
This is the same situation for any and all types of wallets. Be warned that transactions sent while the chain is forked could disappear later. If a transaction disappears, Bitcoins sent would automatically return to the sender. Coins you receive may disappear later! While the situation remains unresolved, other people may thus not accept a transaction as a valid payment. If 'replay protection' is not implemented for a chain fork, a transaction on one chain can (and likely will) be replayed by an anonymous third party on the other chain. This means that sending coins on one chain will likely cause your cloned coins on the other chain to also get sent.

### What should I do?
In the event that a chain fork happens, the safest thing to do is to do nothing and wait for the dust to settle. Theoretically, the situation should resolve quickly - i.e. which of the different chains becomes the dominant chain - but this is not guaranteed. Considering that a transaction with too low of a fee can take extra time until it enters the blockchain, it is advisable to suspend transacting a day or two before a fork is scheduled to occur.

### What will we do?
In general, our goal is to help our customers protect their coins. We try to be neutral and follow the community's lead. In the event a chain fork occurs that is valued by the community, we will do our best to quickly provide a tool that can safely access and send coins on both sides of the chain fork. This may be either directly in our desktop app or by an integration with a third party app. We will provide status updates and instructions on Twitter as needed.


## Segwit2x forks
The Segwit2x fork scheduled to occur 16 November 2017 has been [called off](https://lists.linuxfoundation.org/pipermail/bitcoin-segwit2x/2017-November/000685.html).



## Bitcoin Cash
Continue reading if you had BTC on a BitBox on August 1st, 2017 and would like to access Bitcoin Cash (BCH).

### Claiming Bitcoin Cash
On August 1st 2017, some businesses and Bitcoin miners cloned Bitcoin
to create a new cryptocurrency coin called Bitcoin Cash (BCH).
As a consequence, anyone possessing Bitcoin (BTC) at the time also automatically received BCH.
Two-way replay protection means that BTC and BCH can be used independently from one another.
You can decide to keep BCH or sell it or ignore it as you wish.

The BitBox firmware natively supports Bitcoin Cash, but the Desktop app does not.
The BitBox to be used directly with the third party app <a target="_blank" href="http://www.electroncash.org/">Electron Cash</a>,
a fork of the popular <a target="_blank" href="http://www.electrum.org/">Electrum Bitcoin wallet</a>.

**WARNING:** Electron Cash is a copy of the Electrum code with modifications for BCH.
Please read Electrum's notices <a target="_blank" href="https://electrum.org/bcc.txt">here</a> and
<a target="_blank" href="https://electrum.org/bcc2.txt">here</a> to understand the relationship between Electrum and Electron Cash.
<span class="bold">We have and claim no relationship with Electron Cash. We cannot vouch for the safety of any BCH software or application at this time.</span>

**IMPORTANT:** To access your BCH without compromising your BTC, be sure to first 'split' your coins.
This can be done sending your BTC to a seperate wallet. (Step 1 below)
Only your BTC will move and not your BCH because the BCH blockchain has replay protection.
Wait until the transaction is confirmed on the BTC blockchain.
The BCH remains in your old wallet.

### Step-by-step instructions for accessing your BCH
- Transfer all your Bitcoin (BTC), Ethereum & ERC-20 currently held on your BitBox01 to a different wallet
> This is necessary as in order to claim your BCH you might need to plug the microSD card into your computer, thereby potentially leaking your private keys which means your coins could be at risk. To avoid that risk, you should first empty your wallet before plugging the microSD card into your computer.

- Once you have moved the coins out of your wallet download <a href="http://www.electroncash.org/">Electron Cash</a> and follow the instructions in their app's setup wizard in the following manner:

![alt text]({% link /assets/images/forks/ElectronCash0.png %})

![alt text]({% link /assets/images/forks/ElectronCash1.png %})

![alt text]({% link /assets/images/forks/ElectronCash2.png %})

![alt text]({% link /assets/images/forks/ElectronCash3.png %})

![alt text]({% link /assets/images/forks/ElectronCash4.png %})

![alt text]({% link /assets/images/forks/ElectronCash5.png %})

- Be careful here, you have the enter the Bitcoin coinpath **m/44'/0'/0'**:

![alt text]({% link /assets/images/forks/ElectronCash6.png %})

- After the setup is finished, you are able to spend your BCH.


## Bitcoin Gold
Continue reading this section if you had BTC on a BitBox01 on October 24th, 2017 and would like to access Bitcoin Gold (BTG)

### Claiming Bitcoin Gold
In October 2017, the Bitcoin blockchain was cloned, or "forked",
to create a new cryptocurrency coin called Bitcoin Gold (BTG).
As a consequence, anyone possessing Bitcoin (BTC) at the time also automatically received BTG.
You can decide to keep BTG or sell it or ignore it as you wish.
Some <a target="_blank" href="https://bitcoingold.org/">exchanges</a> will allow trading it.

The BitBox firmware natively supports Bitcoin Gold, but the Desktop app does not and likely will not in the future.
However, Bitcoin Gold can be accessed by exporting your private keys into a third party wallet that does support BTG.
Step-by-step instructions for one possible way to access your BTG follow below.
This example uses the popular <a target="_blank" href="https://electrum.org">Electrum</a> software to display private keys and
the <a target="_blank" href="https://coinomi.com/">Coinomi Android wallet</a> to access the BTG.

**IMPORTANT:** To access your BTG without compromising your BTC, be sure to first 'split' your coins.
This can be done sending your BTC to a seperate wallet. (Step 1 below)
Only your BTC will move and not your BTG because the BTG blockchain has implemented replay protection.
Wait until the transaction is confirmed on the BTC blockchain.
The BTG remains in your old wallet.

**WARNING:** We have and claim no relationship with Bitcoin Gold or any third parties supporting Bitcoin Gold.
We cannot vouch for the safety of any BTG software or application or at this time.
The following instructions are provided for those who wish to access their BTG quickly and are willing to assume the risk of potentially losing coins.


### Step-by-step instructions for accessing your BTG
- Transfer your Bitcoin (BTC), Ethereum & ERC-20 currently held on your BitBox01 to a different wallet
> This is necessary as in order to claim your BTG you need to plug the microSD card into your computer, thereby potentially leaking your private keys which means your coins could be at risk. To avoid that risk, you should first empty your wallet before plugging the microSD card into your computer.

- Once your wallet is empty, plug the microSD card into your computer and open the backup file located in the `digitalbitbox` folder. Then copy the "Wallet seed".


- Open the BitBox01 [backup center]({% link bitbox01/other/backup-center.md %}) and paste the "Wallet seed" into the "wallet backup" field. Then enter your [recovery password]({% link bitbox01/setup.md %}#step-2-understand-the-bitbox01-passwords) (in most cases this is not identical to the normal BitBox01 password) and click "Generate". The backup center will then calculate a list of different private keys.

![alt text]({% link /assets/images/forks/BCH5.png %})

- Open <a target="_blank" href="http://electrum.org/">Electrum Wallet</a> and follow the wizard to restore a wallet. When asked for the private key paste the "Electrum recovery key" shown in the BitBox Backup center.

![alt text]({% link /assets/images/forks/BCH6.png %})

![alt text]({% link /assets/images/forks/Electrum_0.png %})

![alt text]({% link /assets/images/forks/Electrum_1.png %})

![alt text]({% link /assets/images/forks/Electrum_2.png %})

![alt text]({% link /assets/images/forks/Electrum_3.png %})

![alt text]({% link /assets/images/forks/Electrum_4.png %})

![alt text]({% link /assets/images/forks/Electrum_5.png %})

- You will now have restored the Wallet in Electrum but as Electrum can only handle BTC not BTG you need to scan the individual private keys into Coinomi Bitcoin Gold "BTG" wallet by scanning the private key belonging to each used address.
  - In Electrum, go to the Addresses tab. If an Addresses tab is not present, click the menu item View then Show Addresses.
  - Use the "Filter" to view "Used" addresses for both "Receiving" and "Change" options.
  - For each used address, right click on the address and select "Private key".
  - Click the QR code icon in the popup window to display the QR code.

To scan these QR codes into Coinomi, click on the menu icon (the 3 vertical dots) in the top right corner of the Coinomi app and select "Sweep Wallet". You are able to access your BTG **after sweeping all used private keys**.

> Note that a private keys will only hold BTG if it was holding BTC at the time of the chain fork.

![alt text]({% link /assets/images/forks/Electrum_6b.png %})

![alt text]({% link /assets/images/forks/Electrum_6c.png %})
