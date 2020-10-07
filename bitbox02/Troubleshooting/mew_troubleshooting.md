---
layout: default
title: MyEtherWallet
nav_order: 1
has_children: false
parent: Troubleshooting
grand_parent: BitBox02
---

# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

If you are having issues using MyEtherWallet with the BitBox02, please take a look at the list below to find your specific issue and respective fix.

## Prerequisites
- A BitBox02 Multi edition hardware wallet
- The BitBox02 needs to be set up. If it isn't follow [this guide]({% link bitbox02/setup.md %})


## Getting started

### Step 1: Install BitBoxBridge
To use your BitBox02 with web wallets such as MyEtherWallet, you need to download and install the BitBoxBridge. The BitBoxBridge is a program that runs in the background and allows the BitBox02 to communicate with web based wallets.

[Download BitBoxBridge](https://shiftcrypto.ch/download/#bridge)

### Step 2: Start using MyEtherWallet with the BitBox02
- Go to [myetherwallet.com](https://www.myetherwallet.com/)
- Click "Access My Wallet" then choose "Hardware".
- Select "BitBox" and then "BitBox02".
- Unlock your BitBox02 by entering the password on the device.
- When using MyEtherWallet for the first time, you will be prompted with a pairing code. Confirm on your BitBox02 that the pairing code matches and select "continue".
- Now you are ready to start using MyEtherWallet!

**Note:** You will be prompted with a pairing code whenever you use the BitBox02 with a new browser or computer.


> **Safety tip:** Always check the URL of  MyEtherWallet. The URL should be https://www.myetherwallet.com/


## Troubleshooting
If MyEtherWallet shows you an error message, please see if you can find the error in the list below.

| Error message| Proposed solution |
|:-------------|:------------------|
| BitBoxBridge not found | Please make you have downloaded and installed the [BitBoxBridge](https://shiftcrypto.ch/download/#bridge). If it is already installed, make sure it is running by following [these instructions](https://guides.shiftcrypto.ch/bitbox02/Troubleshooting/mew_troubleshooting/#issue-bitboxbridge-not-found).|
| Unlock BitBox02  | Unlock the BitBox02 by entering your password on the device|
| Unexpected error | Disconnect and reconnect the BitBox02 and try again.  |
| Action aborted by user  | You cancelled a process on the BitBox02. Try again.  |
| Your BitBox02 is not initialised | Download and install the [BitBoxApp](https://shiftcrypto.ch/start/) to setup your BitBox02.|
| Please upgrade to the newest firmware using Shift Crypto's BitBoxApp| Your BitBox02 firmware is out of date. Open the BitBoxApp to update the BitBox02 |
| MyEtherWallet does not yet support this version of the firmware. | MyEtherWallet may need to update. Try to [hard refresh](https://fabricdigital.co.nz/blog/how-to-hard-refresh-your-browser-and-clear-cache) when on the MyEtherWallet page. If this does not work, it is possible you need to wait for MyEtherWallet to release an update. |
| Trying to connect from a non-whitelisted origin. |**Attention!** You may be on a phishing site. Please check if the URL is correct. The URL for MyEtherWallet should be https://myetherwallet.com |
| Expected exactly one BitBox02. No or more than one BitBox02 detected. | Please make sure you only have one BitBox02 plugged in at a time. |
| Pairing rejected on device, please try again | Reconnect the BitBox02 and accept the pairing code by clicking the “check mark” on the BitBox02 when prompted. |
| Your BitBox02 is busy. Please close all other wallets and try again. | Close the BitBoxApp. Close any other wallets you may have open using the BitBox02, such as Electrum. |
| Device attestation failed | Reconnect BitBox02 and try again. If you keep getting the warning. Please contact support@shiftcrypto.ch |
| Unsupported BitBox device | MyEtherWallet only supports the BitBox02 Multi edition or the BitBox01. If you are using a BitBox02 Bitcoin-only edition, it is not compatible with MyEtherWallet because it does not support Ethereum. |
| Plug in BitBox02 and choose screen orientation by tapping one of the sides. | Make sure BitBox02 is inserted into USB and powered. Choose orientation of BitBox02 by tapping one of the sides of the device. USB connection is only established after you choose the screen orientation. |

### Issue: BitBoxBridge not found
{: .no_toc }

1. To use MyEtherWallet, you need to download and install the [BitBoxBridge](https://shiftcrypto.ch/download/#bridge)
2. If BitBoxBridge is already installed, make sure service is running by visiting    `http://127.0.0.1:8178/` in your browser.
If the bridge is running you should see something like:
```
BitBoxBridge v1.1.0
    GET /api/info
    GET /api/v1/devices
 GET/WS /api/v1/socket/:socket
 ```
 If the bridge is not running, please follow the instructions below to re-start it.

#### Windows
{: .no_toc }

1. In search bar type **services**
2. Find **bitbox-bridge**
3. Check it’s status.

- If status is empty, right click on bitbox-bridge and click Start
- To make sure the BitBoxBridge starts on boot, right click bitbox-bridge -> properties then select in startup type automatic

#### macOS
{: .no_toc }

1. Open Activity Monitor and search for the service **bitbox-bridge**.
  - If it is not listed there, then the bridge is not running.
2. To restart the BitBoxBridge, select it in Activity Monitor, then click the "x" in the upper left corner. Alternatively do the following:
  -	Open the Terminal
  -	Insert the following commands:
  - To stop the bridge run: `sudo launchctl unload /Library/LaunchDaemons/ch.shiftcrypto.bitboxbridge.plist`
  - To re-start the bridge run: `sudo launchctl load /Library/LaunchDaemons/ch.shiftcrypto.bitboxbridge.plist`


- Log files are in /opt/shiftcrypto/bitbox-bridge/logs

#### Linux:
{: .no_toc }

1. To see the status: `$ systemctl status bitbox-bridge`
- You should see something like:
```
bitbox-bridge.service - Shiftcrypto BitBoxBridge
   Loaded: loaded (/usr/lib/systemd/system/bitbox-bridge.service; enabled; vendor preset: enabled)
   Active: active (running) since Fri 2020-02-07 22:58:31 CET; 24s ago
 Main PID: 4556 (bitbox-bridge)
	Tasks: 6 (limit: 4915)
   Memory: 4.4M
   CGroup: /system.slice/bitbox-bridge.service
       	└─4556 /opt/bitbox-bridge/bin/bitbox-bridge
```
2. To stop the bridge run: `$ sudo systemctl stop bitbox-bridge`
3. To re-start the bridge run: `$ sudo systemctl start bitbox-bridge`






If you are still experiencing issues, please contact support@shiftcrypto.ch
