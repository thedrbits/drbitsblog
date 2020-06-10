---
layout: post
title: Selling your Bitcoin Gold from a Bitcoin Paper Wallet using only an iPhone and Mac
author: Dan Rice
tags: 
---
I have bitcoins stored on paper wallets that I created a few years ago and
wanted to sell the associated bitcoin gold which ended up being more complicated
than anticipated, so I wanted to detail my journey in case it helps others who
may want to do the same.

#### **Private keys are precious**

If you have had a bitcoin paper wallet for any length of time then the paper
wallet contains keys that hold bitcoin, bitcoin cash, and bitcoin gold (amongst
other forks and snapshots). Redeeming and separating these coins presents a
challenge: The private key is the same for each of them, so any software you
expose the private key to could steal all of them.

#### **Move the most valuable and most trusted coin first**

It’s kind of like peeling an onion. First you expose your private key to move
the bitcoins, then bitcoin cash, then bitcoin gold. I used this order because
each step poses more risks of losing your coins, and so moving the coins by
order of value minimizes the odds that coins will be stolen or lost.

First of all, I moved my bitcoins to a new wallet by sweeping them using the iOS
app [Bread Wallet’s import
feature.](https://breadapp.com/support/articles/import-wallet/) This removed the
bitcoins from the paper wallet. You can use any reliable bitcoin wallet to do
this that has a sweep/import feature. Once I confirmed the bitcoins had been
moved, I focused on bitcoin cash. Unfortunately, Bread does not support bitcoin
cash, so I used the iOS [Bitcoin.com wallet to import the bitcoin cash from the
paper
wallet](https://www.bitcoin.com/guides/how-to-access-your-bitcoin-cash-bcc-bch)
just like I had done with Bread and btc.

#### **Finally I had isolated the paper wallet to only bitcoin gold**

Now came the challenging part: Bitcoin gold team security is highly questionable
and I found a number of instances where recommended wallets had stolen funds
from users.
[Here](https://www.bitcoin.com/guides/how-to-access-your-bitcoin-cash-bcc-bch),
[Here](https://fnd.io/#/us/iphone-app/1168568820-bitpie-bitcoin-wallet-by-jiajia-fan),
and
[Here](https://www.coindesk.com/bitcoin-gold-wallet-scam-nets-3-million-illicit-earnings/).

While there was nothing else of value in the paper wallet besides bitcoin gold,
I wanted to do the best I could to not compromise the keys in case a new fork
retroactively gave the keys value, and also I wanted to do my best to make sure
I did not lose my bitcoin gold since it did have some monetary value (~$300USD
per coin at the time of writing). Lastly, I wanted to make sure that I did not
permanently compromise my computer or phone in the process and perhaps lose
other cryptocurrency due to that in the future.

#### **Then it got more complicated than I had expected**

After looking at Bitpie reviews and seeing that a user said it stole their money
on the only English review in the iOS App Store, I decided I could not trust it.
At the time of writing, that is the only [iOS wallet available that
bitcoingold.org lists as compatible](https://bitcoingold.org/downloads/).

Bitcoin gold core wallet currently does not support Mac and they list no
supported Mac wallets at all.

#### **Attempt 1: VMWare Fusion running Linux to install the bitcoin gold core wallet**

I first went down the path of setting up a VMWare Fusion Ubuntu virtual machine
and then attempting to install bitcoin gold core, but I discovered this approach
would take a lot of time and more hard drive space than I was happy with. The
blockchain torrent is over 100GB, so I gave up on that approach.

#### **Attempt 2: Android Emulator on Mac**

I chose [NOX as an Android emulator](https://www.bignox.com/), and downloaded
[Coinomi APK from their website](https://coinomi.com/). After installing NOX and
then installing the Coinomi apk, I was running Coinomi on my mac in NOX and was
able to setup a bitcoin gold wallet for the first time.

#### Success

Once configured I used the “Sweep Wallet” option to move the bitcoin gold off
the paper wallet and into the Coinomi wallet. Unfortunately the camera emulation
in NOX did not work on my mac and so I had to manually type in the paper wallet
private key. Regardless, it worked, and I was almost immediately able to send my
bitcoin gold from Coinomi to my [Bittrex account](https://bittrex.com/) where I
could then sell it for something else.

This article was originally posted on Medium and [can be found here.](https://medium.com/@thedrbits/selling-your-bitcoin-gold-from-a-bitcoin-paper-wallet-using-only-an-iphone-and-mac-b223baf2b7b3)