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

### Linux
- run `lsusb` in the command line.
- You should see an entry that includes "BitBox".

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
