---
layout: post
title: Spectre and Meltdown will steal your cryptocurrency
author: Dan Rice
tags: 
---
{% include image caption="The clock is ticking on your cryptocurrency" name="explode.jpeg"%}
\\
[Spectre](https://spectreattack.com/) and
[Meltdown](https://meltdownattack.com/) do not represent a simple exploit, but
rather **a newly discovered type** of side channel attack that affects all
modern cpus from your smartphone cpu to your computer. The entire computing
world is at risk.

#### **The basics of the attack**

Imagine a person was sitting in a chair just before you walked into a room. When
you walk in the room, they ask you to guess which chair they were sitting in.
While you cannot go back in time and see, you could simply feel the chairs in
the room and find out which one feels warm. This is analogous to a side-channel
attack. The fact that the chair holds heat leaks information. Spectre and
Meltdown show a method of using [something called speculative
execution](https://support.apple.com/en-us/HT208394) to generate side-channel
information. Information is leaked by detecting cpu caching of certain values.
In essence they allow one process to gather data that another process has stored
in memory without permission.

#### **Websites you visit run code on your computer**

Yes, simply visiting a website can trigger a Spectre style attack and do so
invisibly. **You won’t know it’s happening.**

#### These attacks leave limited forensic trace information

Different than the majority of exploit attacks and viruses we see today, Spectre
does not modify binaries on your machine or leave a trail of infected files.
Instead, it affects the CPU cache, so there may be no easy way to even know you
were hit by an attack later or forensically trace it back. Even if the exploit
code is cached and recovered it will be difficult to know what information the
attack yielded.

#### Stealing cryptocurrency is the perfect attack usage

Protecting cryptocurrency is about protecting information: Your private keys.
Reading information is the specific capability of these attacks — A hack could
make off with your private keys and you would not even know it happened till the
cryptocurrency left your account.

#### Cryptocurrency users visit common websites

If you are interested in cryptocurrency you probably visit websites that discuss
them which presents a problem: Even if the website is legitimate and
trustworthy, a simple paid advertisement can run a Spectre attack in your
browser and potentially recover cryptocurrency private keys. Once the keys are
stolen, the cryptocurrency can be transferred without your permission. **There
is more immediate reward to attacking cryptocurrency websites than probably any
other niche pocket of the internet. There is nearly a trillion dollars of value
to extract.**

#### Known attacks are currently in proof-of-concept stage

Since proof-of-concept attacks are available, malicious actors will be crafting
them into real attacks in the coming days, weeks, and months that will get more
sophisticated over time. This could also mean expansion of the attack vectors
beyond what we currently know about.

#### The OS and browser patches released do not solve the problem

Unlike exploits we normally see, the patches released thus far do not completely
solve the problem. First of all, the current patches only close some of the
known holes, not all of them. Secondly, **these attacks represent a new type of
attack, and fixing all the ways they could be exploited may even take years
because we don’t know all the ways they can be exploited yet.**

### What you can do to protect yourself

1.  **Make sure you’re running the latest patches on all your devices.** This
includes your operating system and browser as well, but please keep in mind this
does not plug all the holes.
2.  **Cease usage of any browser-based password managers. Modern browsers have
password tools built in and also allow extensions to store passwords through
services such as Lastpass.** Metamask may also be at risk. Keep your passwords
as far away from your computer’s browser as possible. If you use a secondary
application on your computer to store and save passwords that will make attacks
more difficult. Furthermore, storage on a secondary device will be even more
secure. This could be your phone or something like
[this](https://www.hammacher.com/Product/88840?cm_cat=ProductSEM&cm_pla=AdWordsPLA&source=PRODSEM&gclid=Cj0KCQiA7dHSBRDEARIsAJhAHwgNVdcWlPoEHCyIYALV3iU4ZCEhk_Q1WxoEH-BX2WoKXIsir2eV0UoaApDiEALw_wcB).
3.  **Move your cryptocurrency private keys off of exchanges when you aren’t
actively trading them.** Remember, exchanges are also susceptible to these
attacks and may lose your funds if they are attacked.
4.  **Move cryptocurrency off your computer to paper or hardware wallets like Trezor
or Ledger.** This will protect you against almost all simple javascript attacks
and limit the chances of loss. Hardware wallets may be exploitable, but the
attacks would have to be focused on a particular device and extremely complex.
5.  **Don’t put all your eggs in one basket.** Even if you use hardware wallets,
consider using multiple hardware wallets from different brands and maybe mix in
some paper wallets too. Remember that every storage approach has weaknesses.
[Sometimes you can lose cryptocurrency from purely
bugs](http://www.zdnet.com/article/parity-shakes-up-wallet-audits-but-funds-remain-frozen/)
and so for this reason you should not use a single tool to store all your
assets. Even particular cryptocurrencies may be exploited and you should
consider splitting any cryptocurrency you hold amongst multiple in case a
catastrophic bug occurs in one. Diversify in every direction possible.

\\
This article was originally posted on Medium and [can be found here.](https://medium.com/@thedrbits/spectre-and-meltdown-will-steal-your-cryptocurrency-196fa034e329)