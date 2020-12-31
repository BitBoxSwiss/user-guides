---
layout: default
title: Derivation details
seo_title: BitBox02 - Derivation details
nav_order: 7
has_children: false
parent: Advanced features
grand_parent: BitBox02
description: Find out what derivation scheme the BitBox02 uses.
---
# {{page.title}}
{: .no_toc }

## Bitcoin & Litecoin
- The BitBox02 generates wallet addresses according to BIP32 and BIP44 specifications.
- The BIP32 extended master private key is `m`.
- BIP 44 specifies the following standard:
  - `m / purpose’ / coin_type’ / account’ / change / address_index`

### Purpose field
- Purpose is set as follows:
  - Segwit (P2PSH) = `49’`
  - Native Segwit (P2WPKH) = `84’`

### Coin_type field
- Coin_type is set in accordance to SLIP-44:
- Bitcoin = `0'`
- Testnets = `1’`
- Litecoin = `2'`

### Account field
- The BitBoxApp currently only supports a single account, therefore wallets created via the BitBoxApp will use `0'` for the account field.
- Other wallet apps might allow you manually change the derivation path.
  - In that case it's important that you write down which path you chose.

### Change field
- `0` for normal receive addresses.
- `1` for internally generated change addresses.

### Address field
- Addresses are numbered from index `0` in sequentially increasing manner.

## Ethereum
- Path:  `m / purpose’ / coin_type’ / account’ / address_index`
- The BIP32 extended master private key is `m`.
- Purpose: usually `44'`
- Coin_type: usually `60'`
- Account: usually `0'`
- Address_index: Addresses are numbered from index `0` in sequentially increasing manner.
- Other wallet apps might allow you manually change the derivation path.
  - In that case it's important that you write down which path you chose.
