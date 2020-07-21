---
layout: default
title: Full node support
nav_order: 4
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

* In the sidebar, select Settings > Connect your own full node
* In the field “Enter the endpoint” enter the hostname or ip address and the port, e.g. raspibolt.local:50002
* Click on “Download remote certificate”
* Click “Check”, you should be prompted with the message “Successfully establised a connection”
* Click “Add” to add your server to the list on the top
* Remove the Shift servers to only connect to your own server

## Connecting to your full node via Tor
If you have Tor installed on your computer, you can access your own node remotely over Tor.

* In the sidebar, select Settings > Enable tor proxy
* Enable it and confirm the proxy address (usually the default 127.0.0.1:9050)
* When adding your full node as described above, use your Tor address (e.g. gwdllz5g7vky2q4gr45zGuvopjzf33czreca3a3exosftx72ekppkuqd.onion:50001)
