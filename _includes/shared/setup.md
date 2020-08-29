
## Download the BitBoxApp
In order to set up your {{include.product}} and create your first wallet you need to download the [BitBoxApp](https://shiftcrypto.ch/app/) for your computer or your Android smartphone (beta).


[Download](https://shiftcrypto.ch/start/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }


## Launch the BitBoxApp

Once the download is finished, please install and launch the app.

You should then see a screen that asks you to plug in your {{include.product}}.

![alt text]({% link assets/images/BitBoxApp/BitBox_App_waiting.png %})

{% if include.product == "BitBox02" %}

## Watch the BitBox02 setup video tutorial or continue reading
{: .no_toc }

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/z7nRq2OEhiw' frameborder='0' allowfullscreen></iframe></div>


## Insert microSD card & plug in your {{include.product}}
Before you plug in your {{include.product}}, please **insert the microSD card** which will be needed to create a backup of your wallet in a later step.

{% if include.product == "BitBox02" %}
When done, please plug the {{include.product}} into your computer.
Optional: If needed, use the included USB-C to USB-A adapter and/or USB-C extension cable.
{% elsif include.product == "BitBox01" %}
When done, please plug the {{include.product}} into your computer.
{% endif %}


## Follow the in-app setup wizard

Once the {{include.product}} is plugged in, the setup-wizard will automatically start and guide you through the process of setting up your {{include.product}}.


### Step 1: Choose display orientation
{: .no_toc }
Most laptops have ports on both sides. As we cannot know from which side you will plug your {{include.product}}, you will first need to select your display orientation.

To do that just touch the {{include.product}} on the side that is closer to you.

![alt text]({% link assets/images/BitBox02_wizard/step1.png %})

### Step 2: Confirm pairing code
{: .no_toc }
All information that is exchanged between your computer and the {{include.product}} is encrypted. In order to make sure that there is no man-in-the-middle attack, we need to ask you to confirm that the code on in the BitBoxApp and the code on your {{include.product}} are identical.

Please take the time to check each characters.
![alt text]({% link assets/images/BitBox02_wizard/step2.png %})

If both codes match please confirm on your {{include.product}}. Then click "Continue" in the BitBoxApp.

### Step 3: Create new wallet or restore an existing wallet
{: .no_toc }
Now you are asked to choose if you want to create a new wallet or restore an existing wallet.

![alt text]({% link assets/images/BitBox02_wizard/step3.png %})

- If you already used a {{include.product}} before and you want to restore your wallet from your backup choose "Restore Backup" and follow [this guide]({% link bitbox02/basics/restore-from-backup.md %})

- If you used a different hardware wallet before and you want to restore from the recovery words (seed phrase) created by that other wallet, choose "Restore from recovery words" and follow [this guide]({% link 404.html %}) (TODO)
>**Attention**: The BitBox02 only supports Segwit (starting with 3...) and Native-Segwit (starting with bc1....) accounts. If you import a seed phrase that you used with the Legacy address format (starting with 1...) you won't see these coins in the BitBoxApp. We recommend you to move these coins to a Segwit or Native-Segwit account.

- If this is the first time you create a wallet, choose "Create Wallet" and continue reading this guide.


### Step 4: Create a wallet
{: .no_toc }
First you need to give your wallet a name. This name can be anything, choose a name that you will recognise in the future when you might need to restore from your backup.

If you cannot click the "Continue" button make sure that you have inserted your microSD card into the {{include.product}} correctly and given the wallet a name.
![alt text]({% link assets/images/BitBox02_wizard/step4b.png %})

Please then confirm the wallet name on your {{include.product}}.
![alt text]({% link assets/images/BitBox02_wizard/step4c.png %})

### Step 5: Set your {{include.product}} device password
{: .no_toc }
Next you need to set a device password for your {{include.product}} which you will need to input every time you want to use your {{include.product}}. Please make sure that you remember this password and that it is not easy to guess.

The setup wizard will show you a video of how to use the touch on your BitBox02 to input your password.
![alt text]({% link assets/images/BitBox02_wizard/step5.png %})

### Step 6: Create your wallet backup
{: .no_toc }
After the device password is set, the {{include.product}} will create a backup of your wallet and save it on the microSD card. Please check the boxes to confirm that you understand the security considerations, then click "Continue".

Your {{include.product}} will then ask you to confirm today's date as that is needed for the backup file.

> The backup file on your microSD card is not password protected. That means if someone find your microSD card they can steal your funds. Therefore you should **make sure that you store your microSD card backup in a secure location.** However, you can protect your backup by using the optional [passphrase feature]({% link bitbox02/advanced/passphrase.md %}).

![alt text]({% link assets/images/BitBox02_wizard/step6.png %})

>- You can create multiple backups of your wallet on multiple microSD cards. To do so follow [this guide]({% link bitbox02/basics/managing-backups.md %}#creating-a-new-backup)
- You can at any point check that you still have a valid backup. To do so follow [this guide]({% link bitbox02/basics/managing-backups.md %}#verifying-a-backup.md)

{% elsif include.product == "BitBox01" %}

## Insert microSD card & plug in your {{include.product}}
Before you plug in your {{include.product}}, please **insert the microSD card** which will be needed to create a backup of your wallet in a later step.

{% if include.product == "BitBox02" %}
When done, please plug the {{include.product}} into your computer.
Optional: If needed, use the included USB-C to USB-A adapter and/or USB-C extension cable.
{% elsif include.product == "BitBox01" %}
When done, please plug the {{include.product}} into your computer.
{% endif %}


## Follow the in-app setup wizard

Once the {{include.product}} is plugged in, the setup-wizard will automatically start and guide you through the process of setting up your {{include.product}}.


### Step 1: Create new wallet or restore an existing wallet
{: .no_toc }
Now you are asked to choose if you want to create a new wallet or restores an existing wallet.

- If you already used a {{include.product}} before and you want to restore your wallet from your backup, choose "Restore a wallet from a backup" and follow [this guide]({% link bitbox01/basics/restore-from-backup.md %}).

- If this is the first time you create a wallet, choose "Create a new wallet" and continue with this guide.

![alt text]({% link assets/images/BitBox01_setup/bb01_setup1.png  %})


### Step 2: Understand the {{include.product}} passwords
{: .no_toc }
The {{include.product}} makes use of two passwords:
* A **device password** that you need whenever you want to use your {{include.product}}. This password can be changed later.
* A **recovery password** that protects your backup. This password can **NOT** be changed later.

**Important:** If you lose your {{include.product}} you will need your backup microSD card **AND** the recovery password in order to restore your wallet. **Just the backup microSD card is not enough.**

**Therefore please ensure that you keep your recovery password and backup microSD card safe and accessible.**
![alt text]({% link assets/images/BitBox01_setup/bb01_setup2.png %})

### Step 3: Start the setup process
{: .no_toc }
Read the information and click "Continue"
![alt text]({% link assets/images/BitBox01_setup/bb01_setup3.png %})

### Step 4: Set device password
{: .no_toc }
Now please set and confirm your device password. This password is needed whenever you want to use your {{include.product}}. It can be changed later.

Click "Set device password"
![alt text]({% link assets/images/BitBox01_setup/bb01_setup4.png %})

### Step 5: Create wallet and microSD card backup
{: .no_toc }
Next your wallet will be created. For that your microSD card needs to be inserted, so that the backup file can be saved on it.

If your have not yet inserted a microSD card into your {{ include.product }}, please do so now and click "Set recovery password now".
![alt text]({% link assets/images/BitBox01_setup/bb01_setup5.png %})

### Step 6: Set recovery password
{: .no_toc }
In this step you will set the recovery password that protects your wallet backup on the microSD card.

This password can **NOT** be changed later.

**Important:** If you lose your {{include.product}} you will need your backup microSD card **AND** the recovery password in order to restore your wallet. **Just the backup microSD card is not enough.**

Please also give your wallet a name that you can remember.
![alt text]({% link assets/images/BitBox01_setup/bb01_setup6.png %})
{% endif %}

### Step 7: Start stacking sats
{: .no_toc }
Great! Your {{include.product}} is ready to use. Please make sure that you store your microSD backup in a **secure location.**
>The microSD card is not needed to use your {{ include.product }} in normal use. It is only needed when you want to restore your wallet from your microSD backup. Please store your microSD card in a secure location.
{% if include.product == "BitBox02" %}
![alt text]({% link assets/images/BitBox02_wizard/step7.png %})
{% elsif include.product == "BitBox01" %}
![alt text]({% link assets/images/BitBox01_setup/bb01_setup7.png %})
{% endif %}
