
## Download the BitBoxApp
In order to set up your {{include.product}} and create your first wallet you need to download the [BitBoxApp](https://shiftcrypto.ch/app/) for your computer or your Android smartphone (beta).


[Download](https://shiftcrypto.ch/start/){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }

## Launch the BitBoxApp

Once the download is finished, please install and launch the app.

You should then see a screen that asks you to plug in your {{include.product}}.

![alt text]({% link assets/images/BitBoxApp/BitBox_App_waiting.png %})

{% if include.product == "BitBox01" %}

## Insert microSD card & plug in your {{include.product}}
Before you plug in your {{include.product}}, please **insert the microSD card** which will be needed to create a backup of your wallet in a later step.

{% if include.product == "BitBox01" %}
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

{% if include.product == "BitBox01" %}
![alt text]({% link assets/images/BitBox01_setup/bb01_setup7.png %})
{% endif %}
