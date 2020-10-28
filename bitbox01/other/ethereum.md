---
layout: default
title: Ethereum integration
seo_title: BitBox01 - Ethereum integration
nav_order: 1
has_children: false
parent: Other guides
grand_parent: BitBox01
description: This guide explains how to use your BitBox01 with the popular MyEtherWallet tool.
---
# {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


Safely and simply store Ether on your BitBox01 using the [MyEtherWallet integration](https://www.myetherwallet.com/)

Please make sure you are using the latest firmware.

## Preparing your BitBox01 for use with MyEtherWallet
- If you have used your BitBox01 before, skip to the [next section](#using-myetherwallet-with-your-bitbox01).
- If you just got a new BitBox01 please set it up with the BitBoxApp. See [this guide]({% link bitbox01/setup.md %}). This will generate wallets for both Bitcoin and Ethereum and the same backup on the microSD card will recover both wallets.

> Note: If ['Full 2FA']({% link bitbox01/advanced/pairing.md %}#level-2-full-second-factor-authentication-2fa) is enabled using the desktop app, Ether can be received but **cannot be sent.** This is also the situation for hidden wallets, where full 2FA is always enabled by default. This will be fixed in the future.



## Using MyEtherWallet with your BitBox01
Browser support: Chrome and Opera browsers work without modification. Firefox or Safari work if a browser extension for Universal 2nd Factor (U2F) devices is installed.

1. Visit [https://www.myetherwallet.com/](https://www.myetherwallet.com/)
2. Click "Access My Wallet"

> Do **not** generate a new wallet on MyEtherWallet by clicking 'Create A New Wallet'. This does **not** create a wallet on your BitBox01. Coins sent there will **not** be stored on your BitBox01.

3. Select "Hardware"
4. Select "BitBox" and click "Choose a Hardware"
5. Type in your BitBox01 **device password** and click "Unlock wallet BitBox"
- Optional: Change "HD Derivation Path": This is not necessary if you just want to use Ethereum
6. Select an account (address) you want to access.
7. Agree to the MyEtherWallet Terms.
8. Click "Access My Wallet".


## Receive Ether
You can now deposit Ether to the Address shown.

## Send Ether
Under "Actions" click "Send Transaction" and fill out the transaction details. Then click "Send Transaction" and confirm on your BitBox01.
