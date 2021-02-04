---
layout: default
title: Privacy
seo_title: BitBoxApp - Which details are shared with Shift company servers?
nav_order: 5
has_children: false
parent: BitBoxApp
description: Learn more about what data is shared with the Shift company servers when using the BitBoxApp without your own full node.
redirect_to: https://shiftcrypto.support/help/en-us/14-privacy
---

# {{page.parent}}: {{page.title}}
{: .no_toc }

1. TOC
{:toc}

---
To use your BitBox in the most privacy preserving way we recommend to connect the BitBoxApp to your own node. For instruction see this [guide]({% link bitboxapp/full-node.md %}).

If you use do not connect the BitBoxApp to your own node, it will connect to the default node which is run by Shift.
The Shift server does not log anything related to our customers BitBoxApp usage and never gets access to the extended public keys of your accounts.

Even though we do not persist any logs, we could in theory log the following data:
- The transaction sent (TxID)
- Receive and change addresses up to gap limits, e.g. all used addresses and up to 20 unused addresses
- Client IP address
- Metadata such as date/time of when the app connected to the server
- Sync status: which headers the client is downloading
