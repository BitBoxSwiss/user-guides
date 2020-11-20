
### Bitcoin 101:
{: .no_toc }
{% include glossary/bitcoin_address_reuse_warning.md %}


## Select account

Use the menu on the left to choose the coin (and type) you would like to receive. To activate more coins and types check out [this guide.]({% link bitboxapp/settings.md %}#active-accounts)


---

{% if include.product == "BitBox02" %}
## Watch receive tutorial video or continue reading
{: .no_toc }
<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/x-pwgSQ2aw0' frameborder='0' allowfullscreen></iframe></div>

{% endif %}

## Click receive

Once you have selected the coin, click the "Receive" button in the upper right corner.
![alt text]({% link assets/images/BitBox02_receive/receive1b.png %})


{% if include.product == "BitBox02" %}
## Verify receive address

You will then see the first few characters of a receive address. In order to get the complete address you need to verify it on your {{include.product}} by clicking "Show and verify full address on device".

![alt text]({% link assets/images/BitBox02_receive/receive2.png %})

The address will then be shown on your {{include.product}} and the BitBoxApp at the same time.

### Change to compatible address (Segwit)
If you are using an exchange or wallet that does not support native segwit (bc1...) addresses, click the "change to compatible address (Segwit)" button to get a standard segwit address with a leading 3...

{% endif %}

## Copy or scan address
You can then scan the QR-code or copy the address.

{% if include.product == "BitBox02" %}
Please confirm that the address you scanned with your other wallet and the address shown on your BitBox02 match.

 **Rule:** Always trust your hardware wallet, not the wallet app.
![alt text]({% link assets/images/BitBox02_receive/receive3.png %})
{% elsif include.product == "BitBox01" %}
![alt text]({% link assets/images/BitBox01_random/bb01_receive1.png %})
{% endif %}

## Receive
You can now use this address to send coins to your {{include.product}}. When you want to make another transaction to your {{include.product}} create a new receive address first, don't re-use addresses.
