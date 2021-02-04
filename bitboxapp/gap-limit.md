---
layout: default
title: Gap limits
seo_title: BitBoxApp - How to change the gap limits?
nav_order: 7
has_children: false
parent: BitBoxApp
description: Find out how to change the BitBoxApp gap limits.
redirect_to: https://shiftcrypto.support/help/en-us/15-other
---

# {{page.parent}}: {{page.title}}
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---
In certain circumstances it is necessary to manually increase the gap limits used by the BitBoxApp. Please choose your operating system, which gap limit you would like to increase and run the appropriate command on the command line.

## On Mac and Linux:
- To change the **receive address gap limit** to e.g. 50:

`open -a BitBox.app  --args -gapLimitReceive 50`

- To change the **change address gap limit** to e.g. 50:

`open -a BitBox.app  --args  -gapLimitChange 50`

- To change both, **receive address gap limit and change address gap limit** to e.g. 50:

`open -a BitBox.app  --args -gapLimitReceive 50 -gapLimitChange 50`

## On Windows:
- To change the **receive address gap limit** to e.g. 50:

`.\BitBox.exe -gapLimitReceive 50`

- To change the **change address gap limit** to e.g. 50:

`.\BitBox.exe -gapLimitChange 50`

- To change both, **receive address gap limit and change address gap limit** to e.g. 50:

`.\BitBox.exe -gapLimitReceive 50 -gapLimitChange 50`
