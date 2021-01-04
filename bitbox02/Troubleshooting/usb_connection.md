---
layout: default
title: USB connection
seo_title: BitBox02 - USB connection
nav_order: 2
has_children: false
parent: Troubleshooting
grand_parent: BitBox02
redirect_from: /bitbox02/Troubleshooting/mew_troubleshooting2/
description: Read this guide if you are having USB issues with your BitBox02.
---

# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

If the BitBoxApp on your computer does not detect your BitBox, please try the following:
1. Plug your BitBox in without an adapter or cable if possible.*
2. Try using a different USB port.
3. Try using a different computer or an android phone.

\* The goal is to find out if the adapter is defect or the BitBox itself.

## To check if your computer detects the BitBox at all:

### Mac
- run `ioreg -p IOUSB -l -w 0 | grep "BitBox"` in Terminal.
- You should see an entry that includes "BitBox".

### Windows
1. Open "Device Manager".
2. Go to "Universal Serial Bus".
3. Look for "USB composite device" (there could be multiple).
4. For each of the "USB composite devices":
- right-click and select "Properties".
- in the dropdown select "Hardware Ids".
- if the ID contains "VID_03EB" and "PID_2403" it is a BitBox.

### Linux
- run `lsusb` in the command line.
- You should see an entry that includes "BitBox".
- If the BitBox device is not detected by the app, you may need to manually adjust USB permissions. To do this for most recent distributions, enter the following line in a terminal (sudo access required), then replug the device:
```
printf "SUBSYSTEM==\"usb\", TAG+=\"uaccess\", TAG+=\"udev-acl\", SYMLINK+=\"bitbox02_%%n\", ATTRS{idVendor}==\"03eb\", ATTRS{idProduct}==\"2403\"\n" | sudo tee /etc/udev/rules.d/53-hid-bitbox02.rules > /dev/null && printf "KERNEL==\"hidraw*\", SUBSYSTEM==\"hidraw\", ATTRS{idVendor}==\"03eb\", ATTRS{idProduct}==\"2403\", TAG+=\"uaccess\", TAG+=\"udev-acl\", SYMLINK+=\"bitbox02_%%n\"\n" | sudo tee /etc/udev/rules.d/54-hid-bitbox02.rules > /dev/null
printf "SUBSYSTEM==\"usb\", TAG+=\"uaccess\", TAG+=\"udev-acl\", SYMLINK+=\"dbb%%n\", ATTRS{idVendor}==\"03eb\", ATTRS{idProduct}==\"2402\"\n" | sudo tee /etc/udev/rules.d/51-hid-digitalbitbox.rules > /dev/null && printf "KERNEL==\"hidraw*\", SUBSYSTEM==\"hidraw\", ATTRS{idVendor}==\"03eb\", ATTRS{idProduct}==\"2402\", TAG+=\"uaccess\", TAG+=\"udev-acl\", SYMLINK+=\"dbbf%%n\"\n" | sudo tee /etc/udev/rules.d/52-hid-digitalbitbox.rules > /dev/null
```

- Or, if the above does not work for your distribution, add yourself to the 'plugdev' group (if not already a member; a reboot may be required for some distributions) and enter the following line in a terminal (sudo access required):
```
printf "SUBSYSTEM==\"usb\", SYMLINK+=\"bitbox02_%%n\", GROUP=\"plugdev\", MODE=\"0664\", ATTRS{idVendor}==\"03eb\", ATTRS{idProduct}==\"2403\"\n" | sudo tee /etc/udev/rules.d/53-hid-bitbox02.rules > /dev/null && printf "KERNEL==\"hidraw*\", SUBSYSTEM==\"hidraw\", SYMLINK+=\"bitbox02_%%n\", GROUP=\"plugdev\", MODE=\"0664\", ATTRS{idVendor}==\"03eb\", ATTRS{idProduct}==\"2403\"\n" | sudo tee /etc/udev/rules.d/54-hid-bitbox02.rules > /dev/null
printf "SUBSYSTEM==\"usb\", SYMLINK+=\"dbb%%n\", GROUP=\"plugdev\", MODE=\"0664\", ATTRS{idVendor}==\"03eb\", ATTRS{idProduct}==\"2402\"\n" | sudo tee /etc/udev/rules.d/51-hid-digitalbitbox.rules > /dev/null && printf "KERNEL==\"hidraw*\", SUBSYSTEM==\"hidraw\", SYMLINK+=\"dbbf%%n\", GROUP=\"plugdev\", MODE=\"0664\", ATTRS{idVendor}==\"03eb\", ATTRS{idProduct}==\"2402\"\n" | sudo tee /etc/udev/rules.d/52-hid-digitalbitbox.rules > /dev/null
```
