---
layout: default
title: Address types
seo_title: BitBoxApp - What are unified accounts and what are the different address types?
nav_order: 2
has_children: false
parent: BitBoxApp
description: Learn more about the different address formats available in the BitBoxApp.
redirect_to: https://shiftcrypto.support/help/en-us/13-adresses
---

# {{page.parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

The BitBox Desktop App it supports three Bitcoin transaction formats:
* Legacy — referred to as “Bitcoin Legacy” in the app
* Segwit — referred to as “Bitcoin” in the app
* Bech32 — referred to as “Bitcoin: bech32” in the app


**Info:** If you have upgraded the desktop app from an older version, your bitcoin will appear in the “Bitcoin Legacy” account.



## Legacy format
This account is based on the old transaction format. While upgrading your desktop app, your bitcoin balance and transaction history will be visible here. Now that network fees are relatively low, we recommend moving your bitcoin to the Segwit account at your earliest convenience.

## Segwit format
Also known as “Segregated Witness” is now supported with a dedicated account listed first in the app. It is fully compatible with the bitcoin protocol, and was introduced with a soft fork. It is intended to support more simultaneous transactions, decrease transaction costs , and pave the way for further improvements. It effectively increases the block size limit of the blockchain to improve on-chain scaling.
Perhaps most importantly, Segwit is required to enable the upcoming Lightning network which is designed to reduce transaction speed to milliseconds (from minutes which is the case for bitcoin transactions today). Lightning will significantly increase network capacity by moving the bulk of transactions onto a decentralised second-layer.
In order to reduce your future transaction fees and support the bitcoin network, we recommend moving your legacy bitcoin into the Segwit account and start using it immediately. You can easily do this with the BitBox desktop app: simply generate a receive address in a bitcoin Segwit account and send your coin there from the bitcoin legacy account. In the desktop app, your bitcoin Segwit account is the first one listed. Segwit addresses always start with the number “3”.

## Bech32 format
This is a newer version of the SegWit address format which incurs even lower network fees. Unfortunately it is not yet widely supported so some wallets/services might not let you send to a bech32 address. Its addresses always start with “bc1”. You can receive bitcoin to your Bech32 account from other wallets and services that support Bech32, and you can send bitcoin from your Bech32 account to any address. You can track the progress of Bech32 adoption at bitcoin.it/wiki/Bech32_adoption. Bech32 is not visible in the desktop app by default, to activate it go to the Settings in the lower left corner.


## Unified accounts (since v4.20.0)
Since version 4.20.0 the BitBoxApp unifies the three different Bitcoin account types into one account.
If you want to return to the old behaviour, where each script type is a seperate account go to the BitBoxApp settings and enable "Separate accounts by address type (legacy behavior)".
