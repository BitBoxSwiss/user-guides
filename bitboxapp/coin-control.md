---
layout: default
title: Coin control
seo_title: BitBoxApp - What is coin control and how can I use it?
nav_order: 3
has_children: false
parent: BitBoxApp
description: Find out what coin control is and how to use it when making transactions.
---

# {{page.parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

One of the advanced features of the new BitBoxApp is Coin Control. It adds a privacy enhancing capability by allowing you to choose which unspent transaction outputs(UTXO) you want to use for your transaction.

## Enable coin control
To enable coin control go into the BitBoxApp settings and under "Expert Settings" tick "Enable coin control".
![alt text]({% link assets/images/BitBoxApp/app_settings1.png %})

## Use coin control
### Open the account you want to spend from and click "Send"
{: .no_toc }
![alt text]({% link assets/images/Coin_Control/coin_control1.png %})

### Click "Toggle Coin Control" and select UTXOs
{: .no_toc }
Select the UTXO(s) you want to use as inputs for your transaction.
![alt text]({% link assets/images/Coin_Control/coin_control2.png %})
![alt text]({% link assets/images/Coin_Control/coin_control4.png %})

### Fill out the transaction details
{: .no_toc }
Now just fill out the transaction details as usual. Keep in mind that only the UTXO(s) that you have selected will be used as inputs which means that clicking "Send all" sends the sum of the selected UTXO(s) (minus fees), not your whole account balance.
