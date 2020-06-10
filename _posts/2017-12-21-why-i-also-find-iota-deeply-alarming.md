---
layout: post
title: Why I also find IOTA deeply alarming
author: Dan Rice
tags: 
---
Earlier this year, an Ethereum developer [Nick Johnson wrote a blog with his
thoughts on
IOTA](https://hackernoon.com/why-i-find-iota-deeply-alarming-934f1908194b) that
I agree with, but I wanted to go deeper on a few things.

Let me start off by saying that the price of any asset may not directly
correlate to the technology of the project and I intend to talk about technical
merits of IOTA in this article. The price may go up or down in the future. I
really don’t know. Building a cryptocurrency is largely about community,
ecosystem, and branding — IOTA has excelled at those. Ecosystem is the reason
why Bitcoin has a larger market cap than Litecoin today. Ecosystem is the reason
why if I create a clone of Ethereum today it will probably be worth almost
nothing while Ethereum has a multi-billion dollar market cap. Even if I’m right
and IOTA has fundamental flaws, at some point the IOTA team may just change
technical details of their roadmap and the community may choose to stick with
them; so, there could be long term value there even if the current plan fails.

Myissues with IOTA are not extremely deep in the technicals like the ones [Neha
Narula talked
about](https://medium.com/@neha/cryptographic-vulnerabilities-in-iota-9a6a9ddc4367).
My issues come from the foundations of the cryptocurrency movement and some
specifics that new entrant investors into the space may or may not be aware of.
I want to focus on just a couple areas that raise more questions than answers
for me.

### Unbounded Transactions and Incentives

*“**Incentives matter greatly — underestimate them at your peril. People will
navigate the shortest path to the incentive. The curious among us will pay
particular attention to incentives, monetary or otherwise.**”*

*— Charlie Munger*

Incentives are the key to decentralization. Before Bitcoin, essentially 100% of
monetary online transactions were centralized. Meaning: One centralized bank
account to another. Bitcoin represented an attempt to change that paradigm.

Bitcoin, with its proof-of-work system, attempted to balance incentives of the
parties on the platform in a way that would allow it to function without a bank
being involved or without creating new centralized bank-like entities on the
network. **One extremely important engineering goal of Bitcoin was that a
typical user’s computer should be powerful enough to fully participate in the
network.**

This meant that the network must be constrained to support the following
consumer resource limits:

* CPU Processing Power
* Hard Drive Storage
* Memory
* Internet Bandwidth

### **A common misconception about blocksize**

Bitcoin attempts to limit resource requirements of nodes by limiting the
transaction volume (block size) of the network. A common marketing bullet for
competing cryptocurrencies is that they can handle more transactions than
Bitcoin can handle. A common misunderstanding is that Bitcoin technology is more
antiquated and that is why the transaction volume is more limited. That is not
the case. Bitcoin software can scale to larger transaction volumes with just a
few parameter changes. The constraints on the block size of Bitcoin are self
imposed to maximize node participation and decentralization of the platform.
Every full node on the network must track and store every transaction, so
transactions have a cost. **Transaction volume is a tradeoff.**

As an example, I’ve recently been running the Ethereum blockchain as a part of
our work at Bootstrap Legal. That blockchain can now take up more than 100GB and
[I discovered that due to the network transaction volume, my development
computer is not capable of processing blocks fast enough to keep up with the
network](https://github.com/ethereum/go-ethereum/issues/14895). The solution was
to buy a $300 SSD hard drive to fix this issue and until I get it up and
running, I cannot fully participate in the network. I had to buy special
hardware to stay on the network. With each expanded resource requirement, nodes
will drop off the network who cannot afford to buy the needed hardware.

Now back to IOTA. IOTA has no limit on transactions and therefore, it has no
limit on bandwidth requirements or disk space. It advertises free transactions
with a small amount of proof-of-work. **This means, if you run a full IOTA
node, anyone on the IOTA network can write data to your hard drive with just a
small, extremely low cost proof-of-work. This does not align incentives of the
network for decentralization, but rather centralization.** Over time, the IOTA
transaction set size can grow unbounded, leaving only storage farms with the
resources required to host the data. Not only that, without mining, the storage
farms have no direct network-based economic incentive to host all of this data.
Hosting IOTA transaction history is equivalent to opening a data pipe and
saying, “Internet, send any data you want here and I’ll store it forever.” There
is a reason why companies don’t do that: It does not make economic sense to do
so. It does not align with their incentives.

### IOT and Proof-of-work

Even in name, IOTA describes itself as a cryptocurrency with IOT devices in
mind. My past experience working at companies that develop hardware products
tells me this does not make sense in any other way but a marketing bullet.

To understand hardware devices, you need to understand how important the BOM
(bill of materials) is. The BOM lists every part that needs to be put into a
device that will be built. It is the cost basis for the device itself and it is
a fixed cost for every unit you produce. This means not just dollars, but
pennies add up when you build a lot of units. Inside a company, what happens is,
you build a prototype of a hardware device and normally the BOM is initially
very high. You build just a few for internal use at the company, and then you go
to work cutting everything you can. Every chip, every capacitor, you ask
yourself, “Do we really need this or is there some way we can remove it or use a
cheaper one?”

You do the exact same thing with power consumption of any product that relies on
batteries as many IOT devices do.

IOTA claims their Ternary-based Proof-of-Work function will work with IOT
because it uses minimal power, but I contend that any power usage more
significant than signing a transaction is too much because there is another
alternative approach. For any proof-of-work cryptocurrency, mining represents
the function that creates this scarce resource currency. The cool part about it
is that you can do the work at an earlier time, but use the currency later.
Likewise, when you buy Bitcoin or Ether you’re outsourcing the work to a miner
and exchanging fiat with them in exchange for them doing the work for you.
Someone mined that currency using work. An IOT device that is power consumption
limited can be more efficient without IOTA by owning its own private keys and
holding a small amount of cryptocurrency that it can use to transact on the
network if it really needs to do that.

### Do IOT devices need to connect to public blockchains?

There are many ways an IOT device can participate on a cryptocurrency network
and running a node is only one of those methods. First of all, practically zero
IOT devices will have the resources to act as a full node on a public
cryptocurrency network. Even without storage requirements, how do you feel to
know that your fridge is using 99% of your internet bandwidth because it is
acting as a node on the IOTA network listening and relaying transactions? Most
people do not want to worry about that.

**IOT devices will use public cryptocurrency networks in the lightest way
possible to limit their BOM and their power usage.** The minimum could be one of
the following:

1.  Contacting a central server run by the company that built the IOT device,
announcing the need to submit a transaction at which point the centralized
server will submit the transaction on the device’s behalf.
1.  Contacting the cryptocurrency network momentarily only to submit a signed
transactionusing the private key stored on the device.

[Remember 21 Inc already tried to do the proof-of-work on device thing, and they
have since
pivoted.](https://siliconangle.com/blog/2015/09/24/21-inc-changing-the-way-we-pay-for-and-play-with-the-internet-of-things/)

This does not address listening. If for any reason an IOT device wants to be
aware of particular transactions sent by other devices on a cryptocurrency
network, it will want to filter for only those messages and that may require a
centralized company node to filter those and pass them on to the listening
device. In other words, connecting directly would not be a practical idea
considering the network transaction volume is unbounded. In the case of IOTA the
client software design intends to kick nodes off the network that do not
participate enough, so being even just a passive listener is not an option. [“If
one particular node is “too lazy”, it will be dropped by its
neighbors.”](https://iota.org/IOTA_Whitepaper.pdf)

### Incentives back in focus

In spite of my assessment, I do think that IOTA could have value in some areas,
just not as designed today and not as a competitor to public decentralized
blockchains. I suspect that if IOTA has in the past, or does in the future make
any inroads with large corporate entities, they would do so because they see
value in the use of some of this technology in a more controlled setting.
Example: A cooperative local network within a home limited to only permissioned
devices and no proof-of-work. It’s not clear to me how that would create value
for IOTA investors, if at all.

Properly aligned incentives will continue to drive real adoption vs speculation
and at this point cryptocurrency investing is investing in future potential no
matter who you are. The space is very young still and that can make it hard to
separate hype from true innovation. I don’t believe any cryptocurrency is truly
consumer ready, but some are much closer than others and we should keep that in
mind.

This article was originally posted on Medium and [can be found here.](https://medium.com/@thedrbits/why-i-also-find-iota-deeply-alarming-99d4f2da3282)