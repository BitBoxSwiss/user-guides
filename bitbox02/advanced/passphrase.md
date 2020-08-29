---
layout: default
title: Optional passphrase
nav_order: 3
parent: Advanced features
grand_parent: BitBox02
---

# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---
## How it works
Simplified: When you set up a BitBox02, it  generates a "long random number" which is converted into your 24 recovery words (also called mnemonic seed), which is  stored on the device and on the microSD card backup.

Subsequently, whenever the BitBox02 is used, it derives a cryptocurrency wallet via a (very simplified) formula:
**recovery words + passphrase -> wallet**

If you don't use a passphrase that is: 24 recovery words + "" (empty string)

If you use a passphrase that passphrase is appended to the recovery words and your wallet is derived from that.

As a result to how that process works, **any passphrase is *valid***. Valid in the sense that you won't get an error message but if the passphrase is not identical to the one you used when you set up your wallet, you will derive a different wallet.
### Example:
{: .no_toc }

recovery words + passphrase1 -> wallet1

recovery words + passphrase2 -> wallet2

recovery words + passphrase3 -> wallet3

### Attention: Any passphrase is valid
Mistyping the passphrase will generate a completely new wallet. There is no such thing as an "incorrect passphrase", so whatever you provide as your input will be used in the process of deriving a wallet.

If you enter an empty passphrase (no passphrase at all), your BitBox02 will proceed exactly as if the passphrase feature had not been activated at all and derives a wallet from only your recovery words which are stored on the device.

> **In order to restore a wallet that used a passphrase you will need your backup (stored on microSD card) AND the passphrase you used for that wallet.**


### Benefits of using a passphrase
1. Because the passphrase is not stored anywhere on the device, it helps to protect against any attacks involving physical access to the device. Furthermore, if somebody compromised your physical copy of the recovery words (i.e. your microSD card backup or the recovery words written down on paper (optional)), they still would not be able to access your wallet unless they also know the passphrase.
2. You can create as many passphrase-protected wallets as you like. This gives you a secondary advantage: hidden wallets = plausible deniability.
>Example: You might want to leave some pocket money in the basic "non-passphrase" wallet, then move a portion of your funds to one passphrase; and lastly, the most significant portion of your funds to another passphrase-protected wallet.
The idea behind this is that if you ever find yourself in a situation where somebody is trying to extort a ransom from you or puts you under duress, you can safely give up the PIN.

### Risks of using a passphrase
1. Because the passphrase is not stored anywhere automatically, you need to take **all necessary precautions** in order to make sure that the passphrase stays safe and accessible e.g. by making a physical backup.
2. If the passphrase is lost, you will not be able to access that wallet anymore and any coins stored in that wallet will become unaccessible.

## Using a passhrase
### Enable optional passphrase in device settings
Go to "Device settings" and click "Enable optional passphrase".
![alt text]({% link assets/images/BitBox02_passphrase/passphrase1.png %})

You will then see the following warning
![alt text]({% link assets/images/BitBox02_passphrase/passphrase2.png %})

Please make sure you understand how a passphrase works. If that is the case, confirm on your BitBox02 that you want to enable it.

Then you will see the following:
![alt text]({% link assets/images/BitBox02_passphrase/passphrase3.png %})

From now on you will be asked for a passphrase after every device unlock.
- If you want to use your "normal" wallet just confirm directly i.e. with no passphrase input / empty passphrase.

- If you want to access a passphrase-protected wallet, type in the corresponding passphrase and then confirm.

### Pro tip: hiding that you are using a passphrase
If you don't want to be asked for your passphrase every time you unlock your BitBox02 you can click "Disable optional passphrase" at any time in the device settings. As no data about your passphrase is stored on the device (you need to backup your passphrase independently) nothing is deleted. If you want to use the passphrase-protected wallet again you can just "Enable optional passphrase" again and then use the same passphrase again to access that wallet.
