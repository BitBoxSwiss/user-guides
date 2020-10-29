---
layout: default
title: Reproducible builds
seo_title: BitBox02 - What are reproducible builds?
parent: Advanced features
grand_parent: BitBox02
nav_order: 4
description: Learn more about reproducible builds and why they are important.
---
# {{page.grand_parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---

## Why reproducible builds?
Whilst anyone can inspect the source code of open source software for malicious flaws how can you be certain that the binary built from that public source code is actually on your device?

Reproducible builds, also known as deterministic compilation, is a process of compiling firmware in a way that is reproducible, i.e. results in the exact same binary. By building the binary yourself and comparing the resulting checksum to the one we calculated you confirm that the binaries are identical.

## What you can do
Please follow the README in the BitBox02 firmware repository: [https://github.com/digitalbitbox/bitbox02-firmware/tree/master/releases](https://github.com/digitalbitbox/bitbox02-firmware/tree/master/releases)
