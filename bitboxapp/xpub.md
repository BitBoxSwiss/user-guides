---
layout: default
title: Extended public key
seo_title: BitBoxApp - How to access my wallet extended public key?
nav_order: 3
has_children: false
parent: BitBoxApp
description: Find out how to access the extended public key of your BitBox02 wallet.
redirect_to: https://shiftcrypto.support/help/en-us/13-adresses
---

# {{page.parent}}: {{page.title}}
{: .no_toc }

1. TOC
{:toc}

---
## What is an extended public key?
The extended public key (xpub) is the master public key of a cryptocurrency account. All account addresses are mathematically derived from this key.
That means that if you share your extended public key, the recipient can create all the addresses of your account, which is bad for your privacy.
As the name suggests it's a public key, meaning you can only view transaction details but not make transactions using an extended public key.

## How many extended public keys do I have?
There is one extended public key for each account in the BitBoxApp. Some coins, for example Bitcoin have multiple script types, which means that these coins also have multiple extended public keys.

## How to display the extended public key?
In order to access the extended public key of an account, click on the "Account info" button in the upper right corner. You will then see all the extended public keys that are associated with that account in the form of a QR code and the plaintext key below.

In most cases that is just one extended public key, but for example if you use the "unified accounts" feature you will see multiple extended public keys.

![alt text]({% link assets/images/BitBoxApp/account_info.png %})
