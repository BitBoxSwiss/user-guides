---
layout: default
title: Full node support
seo_title: BitBoxApp - Why should I run my own full node and how can I connect my BitBoxApp to it?
nav_order: 4
has_children: false
parent: BitBoxApp
description: Learn more about why running a full node is important and how you can connect your full node to your BitBoxApp.
---

# {{page.parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Why should I run my own node?
Running your own node is not necessary but improves privacy and reduces the need to trust others.
Firstly, it means that you are using Bitcoin more privately as the BitBoxApp won't connect to our servers to fetch your transaction history; instead it will fetch that information from your own node.
Secondly, running your own node means that your node verifies all transactions itself, making sure that the consensus rules are enforced.

## What options are there to run a node?
There are multiple options to run your own node such as buying a finished device, building your own or running Bitcoin Core.
If you want to connect your BitBoxApp to your node, make sure that it runs an Electrum server. This is a dedicated program that allows a wallet app to communicate with your full node.
The BitBoxApp supports Electrs, Electrum Personal Server (EPS) or Bitcoin Wallet Tracker (BTW).

## Should I use clearnet TCP, TLS or Tor?
If you intend to only connect to your node when you are on the same network (e.g. your home wifi), then using regular network communication is sufficient.
In this case it is advisable that your Electrum server provides a TLS certificate to encrypt the communication.
If you intend to connect to your node from anywhere, using Tor is the better option. No TLS certificate is necessary in that case.

## What is Tor, Tor proxy and which port should I use?
Tor stands for 'The Onion Router', which is a free and open source software that offers a lot of privacy benefits and is especially useful when using Bitcoin.
If you intend to connect to your node via Tor, make sure that Tor is installed on your computer and then enable the Tor Proxy in the BitBoxApp settings.
On most operating systems there are two ways to run Tor:
1. Tor Browser: download and open the Tor Browser. This will allow the BitBoxApp to connect to the Tor network by setting port 9150 in the Tor proxy settings.
2. Tor background service: install the Tor daemon, which always runs in the background. The BitBoxApp can then connect by setting port 9050 in the Tor proxy settings.

## Connecting to your full node without Tor
On your regular computer, configure the BitBoxApp to use your own node:

1. In the BitBoxApp sidebar, select Settings > Connect your own full node.
3. In the field “Enter the endpoint” enter the hostname or ip address and the port. For example `blockstream.info:700`.
4. Click on “Download remote certificate”.
5. Click “Check”, you should be prompted with the message “Successfully established a connection”.
6. Click “Add” to add your node to the node list at the top of the page.
7. Remove the Shift servers if you want to only connect to your own node.

## Connecting to your full node via Tor
If you have Tor installed on your computer, you can access your own node remotely over Tor.
- Instead of an IP address and port use your nodes's TOR address and port. For example `gwdllz5g7vky2q4gr45zGuvopjzf33czreca3a3exosftx72ekppkuqd.onion:50001`.
- When using TOR you **don't** need to download a remote certificate so skip step 4.
- In the BitBoxApp sidebar, select Settings > Enable tor proxy.
- Enable the proxy and confirm the proxy address.
  - If you are running the TOR deamon it probably is: `127.0.0.1:9050`
  - If you are running the TOR browser it probably is: `127.0.0.1:9150`
- Then restart the BitBoxApp in order for the new settings to take effect.
