---
layout: default
title: Settings
nav_order: 6
has_children: false
parent: BitBoxApp

---

# {{page.parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---
![alt text]({% link assets/images/BitBoxApp/app_settings1.png %})

The BitBoxApp currently has three settings sections:

## Currencies
Here you can select which Fiat currencies should be available in the App. If you have multiple selected you can switch between them by clicking on the Fiat currency short-code (such as "USD") on the transaction history page.

## Active accounts
This section lets you choose which coins and coin-types should be enabled in your BitBoxApp.
If you are new we would recommend to avoid Legacy and if possible prefer the Bech32 accounts as these have the lowest fees.

All activated accounts show up in the left menu bar:
![alt text]({% link assets/images/BitBoxApp/app_side_bar.png %})


### Troubleshooting: "My coins are gone after BitBoxApp update"
If you upgraded your BitBoxApp please enable all coin types and check if you can now find your coins again. You might have used an account type that is not enabled by default.

All activated accounts show up in the left menu bar. Please check each of these accounts, make sure you are connected to the internet and wait a few seconds for the app to load your transactions.
![alt text]({% link assets/images/BitBoxApp/app_side_bar.png %})


## Expert settings
In this section you can enable [Coin control]({% link bitboxapp/coin-control.md %}) connect the BitBoxApp to [your own full node.]({% link bitboxapp/full-node.md %})
