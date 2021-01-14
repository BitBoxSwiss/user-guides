---
layout: default
title: Export wallet
seo_title: BitBox02 - How to export a BitBox02 wallet?
nav_order: 7
parent: Basic features
grand_parent: BitBox02
description: Find out how to export a BitBox02 wallet into a third-party hardware wallet.
---

# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

Find the right section for your circumstances:
- Your wallet was created on a BitBox02:
  - [You want to import your wallet from your microSD card backup]({% link bitbox02/basics/import-wallet.md %}#import-wallet-from-microsd-card-backup)
  - [You want to import your wallet from your 24 recovery words]({% link bitbox02/basics/import-wallet.md %}#import-wallet-from-recovery-words)
- Your wallet was not created on a BitBox02:
  - [You want to import your wallet from your 24 recovery words created by a different wallet]({% link bitbox02/basics/import-wallet.md %}#import-wallet-from-recovery-words)
- You lost your BitBox02 and want to export your BitBox02 wallet into a different hardware wallet:
  - [You want to export your BitBox02 wallet into a different wallet]({% link bitbox02/basics/export-wallet.md %}#export-bitbox02-wallet-into-third-party-wallet)


## Export BitBox02 wallet into third-party wallet
- This section explains how you can import your BitBox02 wallet into a different hardware wallet.
- This is important in case you loose your BitBox02 and cannot get access to a new BitBox02.
- We recommend to only import a wallet created with a BitBox02 on another hardware wallet.
 - Do not import it in a software wallet such as on a computer or smartphone.

### Export wallet using microSD card backup
- Before you can use your wallet backup contained in your microSD card backup you first need to extract the 24 recovery words from it.
- For that you can use our [backup recovery tool]({% link bitbox02/advanced/backup-recovery.md %}).
- The backup recovery tool is run on your computer which could potentially leak your wallet.
- Read the advice on the backup recovery tool page carefully.
- You should **only use the backup recovery tool if absolutely necessary**, meaning you cannot get access to a new BitBox02 and you do not have [your 24 recovery words]({% link bitbox02/advanced/view-seed.md %}) written down.

### Export wallet using 24 recovery words
- You can use this option if you have [written down your 24 recovery words]({% link bitbox02/advanced/view-seed.md %}).
- You can then just click "restore" on your new hardware wallet and enter the 24 recovery words to restore your wallet.
