---
layout: post
title: Ethereum Transaction Fees Hamper Adoption
author: Dan Rice
tags: 
---
{% include image name="1.jpeg"%}
As a co-founder of a company that is building smart contracts and using blockchains, I spend a lot of time thinking about market traction. As I have researched companies that raised ICOs a couple of years ago, I’ve been appalled to find that very few of them have a focus on practical usability at all, and thus traction. There are a couple of different philosophies that can guide a crypto-space project in regards to traction.

One is to build and integrate into the existing blockchain ecosystem with the mentality “if you build it they will come”, meaning some teams do not see their project as a direct driver to adoption of cryptocurrency, but rather a tool to be available for those that enter the market. A lot of ICO infrastructure projects fall into this camp. “We are building a decentralized exchange on Ethereum” was the ICO whitepaper pitch, so the team goes and starts building that exact system. In these cases, there may even be a legal obligation to execute the plan that was originally promised in the whitepaper since people gave money with a particular assumption of what would be built. The danger of this approach is that the company ties their success to the adoption of the platform the project is being built on. Furthermore, the team may not have the ability to respond to changes in the ecosystem that require them to pivot their original concept.

The second approach to building a cryptocurrency project is to act more like a traditional startup, meaning: Build a minimum viable product, solve an urgent problem with large market potential, get it in front of customers fast, and iterate. This approach means looking for ways to be the driver of ecosystem adoption rather than tying success to a single blockchain platform. If your company can entice new users to make first contact with your system, they may have to overcome special hurdles required by the protocol your system is built on. For this reason, it’s important that we closely analyze what hurdles exist to new user adoption of these platforms, and that we evaluate whether certain protocols are more user-friendly than others.

There are many different ways to look at the usability of a platform, but for this article I want to focus in on transaction fees and specifically those of Ethereum. I’m focusing on Ethereum because it’s the most popular public smart contract protocol.
<br>
<br>
#### **Generalizing Cryptocurrency Transaction Fees**

There are several models around cryptocurrency transaction fees, but the same basic model is present in both of the two largest cryptocurrencies by market cap: Bitcoin and Ethereum. Ethereum transaction fees are called gas fees because the virtual machine can execute Turing complete code and needs a way to decide when to stop executing that code due to something called the halting problem.

The general model follows what I consider to be the most obvious solution: If you want to use the network (i.e. make a transaction), then you need to pay for that transaction. It is a very direct solution to a direct problem. Someone needs to pay for network usage, so why not just charge the fee directly to the person trying to use it?
<br>
<br>
#### **Direct Transaction Fees Deter Usage**
{% include image name="2.jpeg"%}

One reason to not charge direct fees is the visibility of the transaction cost. Credit cards charge a transaction fee that is typically around 3% of the transaction. This fee is not directly charged to the buyer, but rather the seller. Credit card processing merchant contracts also generally prohibit the seller from charging a markup on credit card purchases, and this means the buyer pays the same price whether or not they use a credit card. Buyers do in fact pay a fee for credit card usage, because the seller must bake that fee into their prices, but that fee is charged whether or not the buyer pays with a credit card, and that means it’s only indirectly related to the fee the seller pays for credit card processing. Charging transaction fees to the buyer indirectly is psychologically and practically very different than charging them directly. Charging directly for credit cards would mean the customer at the checkout would pay a higher price when using a credit card than with cash and that means at every checkout they would ask themselves, “Should I pay with cash and pay less, or should I pay with credit and pay more?” Ask yourself if you think credit cards would be as common today if they were always more expensive at the register than cash.

***Users will use a paid solution only if a reasonably comparable free solution does not exist.***
<br>
<br>
#### **Lessons from Mobile**
{% include image name="3.jpeg"%}

***microtransaction — a very small financial transaction conducted online.***

***micropayment — a very small payment made online.***

I started building smartphone apps as soon as Apple launched the App Store in 2008. In order to make sure that my time was well-spent and that I launched apps in a way that would make them successful, I did a lot of research around business models over those first key years as the world collectively explored what robust apps in our pocket would mean. Mobile was one of the first places we saw digital micropayments tested on a wide scale, and there were very distinct sales patterns that occurred in those early years:

Initially when the iOS App Store launched, several apps charging $.99 or more were the top-grossing apps. Since there was little competition at launch, this was a natural starting place.

As the market expanded, competitive free alternatives with in-app purchases launched in most categories.

Statistics were gathered by developers that showed the majority of smartphone users would not pay any money for a phone app up front. They only used free apps. When developers started to launch free lite and paid full-featured apps side-by-side, they discovered that users would download the free version over the paid version usually at a ratio of roughly 20:1 or greater.
<br>
<br>
#### **Microtransactions Stress the User**
{% include image name="4.jpeg"%}

These smartphone app purchases we are discussing have a unique characteristic in common with cryptocurrency transactions: They are generally small, repeated microtransactions. Beyond the first phase of mobile, moving from paid to free, the next stage focused on something new: If most users were not willing to pay anything, then they would always use the free version, but what about the users who were willing to pay? How much were they willing to pay and what would the optimal model be for a mobile app to make the most revenue? Most mobile apps, when they went from paid $.99 to free with in-app-purchase features, generally just asked users to pay the $.99 to get the added paid functionality. This presented a problem because the apps and companies were supporting 20 times the number of users but making the same revenue as they were before they started to support free users. In reality, some paid users were willing to spend a lot more than $.99 on an app, and so app developers were forced to ask how best to extract the most money from these “whale” users.

Over time app developers discovered that it was a bad idea to ask a user who was willing to spend $100 on an app to spend $.99 one hundred one times. Instead, these companies realized they could offer price-insensitive users bulk packages at any price they were willing to spend, collecting the money in one pass, and leaving the user unworried about spending more. Bitcoin and Ethereum transaction fees follow the repeated small fee model, asking the user at every point, “are you willing to spend a little more?”

In hindsight, it sounds obvious that asking a user to spend $.99 one hundred one times would not be comfortable vs just asking for a lump sum in one transaction, but at the time it was not so clear how best to handle these scenarios. Coincidentally, Nick Szabo, of Cypherpunk and Bitgold fame wrote a very interesting paper on why micropayments will not work well in practice. Constantly asking the user to make a choice about whether or not they want to spend money will tax them mentally.

In 2019 there is almost complete consensus that “whaling” is the best method of collecting revenue from a mobile app, meaning, assume that most users will never pay anything, and collect money in bulk from the biggest users.
<br>
<br>
#### **ICO Tokens as Micropayments**

Over the last few years we saw a great rise in Initial Coin Offerings, particularly on the Ethereum network. Many of these ICOs were selling what they describe as utility tokens. This simply means that the token provides a use, beyond investment, on the network. The most common token use for a utility token is service access, similar to how transactions work on Ethereum: Each individual instance of service use requires a micropayment of the specified utility token. Also note that these Ethereum network transactions require Ether for gas as well, so, in the case of ERC20 they are in effect saying, “In order to use this service you must provide a micropayment of Ether and our ICO token with the transaction” — A double micropayment.

In addition to the complexity of a double transaction fee, both the ETH gas and the ERC20 token have unique and (sometimes wildly) fluctuating exchange rates versus the US Dollar and all other sovereign currencies. This creates additional mental overhead for the user in order to fully grasp the cost of the transaction.
<br>
<br>
#### **Micropayments Ignore Bulk Discount Concepts**
{% include image name="5.jpeg"%}

If I want to buy candy that I plan to eat later at my house, I’m generally not going to collect them in hand-fulls from the vending bubble gum style machine in front of the grocery store because I know that the larger pack inside the store carries a bulk discount. This same concept tends to apply in software as well. Going back to the whaling concept discussed on mobile, as a company you want to incentivize your most valuable users to spend the most money possible and one of the approaches you can use is to offer bulk discounts. If you want a single game power-up, that’s $.99, but if you want ten power-ups, that’s $4.99. This is a standard SaaS pricing model concept as well: “Under 5 users — $100 a month, 5 to 20 users — $75 a month, more than 20 — CALL US.” Companies have learned almost universally that you want to incentivize bulk sales, and offering bulk discounts is a good way to do that.

Bitcoin, Ethereum, and utility tokens have a limited concept of bulk discounting called transaction batching, but that only cuts down the cost of certain transaction types. Users will generally have no added incentive to utilize the network more than absolutely necessary.
<br>
<br>
#### **Variable Microtransaction Fees are Insane**
{% include image name="6.jpeg"%}

There is only one model I can think of that is unquestionably worse than micropayments and that is variable price micropayments. How would you feel about Paypal if they charged you on some days a 1% fee and on other days a 120% fee on a $50 transfer? Sounds insane right? That is exactly what we have seen happen on both the Bitcoin and the Ethereum network. Bitcoin and Ethereum use a transaction fee model where your transaction fee is essentially bidding for bandwidth on the network. The networks have a limited capacity, so in order to discover which transactions should be accepted into that limited space, miners compare fees and generally accept those who pay more. This means the transaction fees on both Bitcoin and Ethereum depend on how busy the network is at the time. At the end of 2017, the transaction fees on both networks saw a dramatic increase, Bitcoin peaked at an average of $50–$60. Scaling solutions like payment channels do give the network more capacity which creates lower fees, but the fees are still load-based and variable.

It’s important to note that Ethereum transactions are also variable in price on a second dimension in that most Ethereum clients cannot correctly pre-calculate the code paths that will be run by a transaction. Since Ethereum transactions are billed based on each code instruction having its own cost, a transaction is submitted with a maximum spend that the transaction will allow. If the transaction ends up being more expensive than the maximum provided, the transaction will not be executed. This also can add to confusion and uncertainty around transaction fees.

The natural impact of variable fees is that, at a certain price, users will cease to use the network and start to look for alternatives. Furthermore, the knowledge that this type of price variability is possible will lead developers to avoid the creation of systems that rely heavily on the variable fee network in the first place. These conclusions have far reaching consequences for both the Bitcoin and Ethereum networks themselves, but also ICOs. When a team considers integration with another project, they must have a deep understanding of how the cost of integration could change over time. Integration with a utility token requires an economic due diligence analysis of the underlying infrastructure associated with that particular token. Typically, in software, if two projects are integrated, they may be decoupled later, but many cryptocurrency projects have a goal of creating an unchangeable system where the software protocol is no longer updated. This makes relying on a separate project with a separate economic model extremely risky because if one project’s economic model becomes unstable, all connected projects will suffer. It is for this reason that a team must deeply understand what could happen to the token transaction price in the future and be sure that it is sustainable under all possible conditions.
<br>
<br>
#### **Separating Currency Transactions**

One distinction should probably be made regarding transaction types on cryptocurrency networks. Bitcoin is generally used as a currency network, meaning the vast majority of transactions are used to transfer value and that is the intent of the network. Ethereum on the other hand goes far beyond value transfer and into the realm of general code execution. Crypto Kitties, as an example, offers transaction functions for mating your kitty with other kitties as a part of the larger game. Many Ethereum transactions may not contain a direct monetary relationship. Transaction fees on non-currency transactions are a fundamentally different proposition. If I buy a toy at my local toy store, and tax is added as a fee to the transaction, it simply means I must provide a little extra money. My general order of operations have not been altered by the requirement for extra funds. Conversely in a non-currency transaction, the request for currency is an added step in my order of operations and adds a new complexity to the exchange. Utility tokens double down on this concept. To call a non-monetary function on Ethereum I may need ETH for gas costs plus utility tokens for infrastructure that will be called during the execution.

While this may not matter greatly for an Ethereum native, it creates an incredibly large hurdle for general adoption. In software we often track potential new users through what we call a funnel. The idea behind a funnel is that at some point a user makes first contact with your company, perhaps by visiting your website. You now track their interaction from that point forward, all the way to the point that they make a transaction. What we find with funnels is that every step in the process, some percentage of users will get distracted and leave. We do not necessarily know why the user left, but we can record in percentages how many left at each stage. For example, if a user is asked to enter their email address and create a password before moving on to the next step, a large percentage will just leave. This has led many companies to create paths that entice users to stay before they are asked to create an account. Medium is an example of this. I can read content for free, but if I want to create content, I will need to take extra steps. Most users probably decide to create a Medium account only after visiting Medium many times. This is very similar to the free vs paid mobile app concept: Provide me value as a user, and I will return the favor.

For cryptocurrency we must take a close look at what barriers these micropayments are creating. If my first intro to Ethereum is a game that a friend tells me about that uses utility tokens, here are the current funnel steps I must complete to play the game for the first time(assuming it’s a DApp):

1. Go to game website
1. Realize you need this cryptocurrency thing and go study up on it
1. Install Metamask
1. Create password
1. Save seed key
1. Create backup copy of seed key in case one is lost
1. Find a safe place to hide my seed key and backups
1. Find a cryptocurrency exchange
1. Create an account on the cryptocurrency exchange
1. Upload photo ID, personal info, and wait for KYC verification (probably days)
1. Connect a bank account, and transfer some money into the exchange
1. Wait for the money to transfer (probably days)
1. Purchase ETH
1. Send ETH to Metamask address
1. Find exchange that supports the correct utility tokens
1. Create an account on the cryptocurrency exchange
1. Upload photo ID, personal info, and wait for KYC verification (probably days)
1. If the utility token exchange supports ETH, then transfer ETH to the new exchange
1. If the new exchange only supports BTC, go back to bank account funded exchange and buy some BTC
1. Send BTC to utility token exchange
1. Convert BTC/ETH to utility token at market price
1. Send utility token to Metamask
1. Go back to game and complete their signup process
1. PLAY!!! WE MADE IT!!!***

That seems like an awful lot to ask of a user and more than a user will probably be willing to do unless they have a massive incentive to complete the process.
<br>
<br>
#### **Scale Matters a Little**

The promise of payment channels like Lighting Network on Bitcoin or other Ethereum scaling solutions like Plasma is that they will make transactions cheaper, but also stabilize the transaction price. Since these technologies increase the transaction throughput of the network, the price per transaction should fall and also the transaction fee range should display lower volatility. This does make the situation somewhat better because it creates more cost predictability, but unless that cost is zero, it still includes a microtransaction.
<br>
<br>
#### **Free Transactions and Cryptocurrency**

The alternative to paid transactions is direct free transactions and they do actually exist. Outside of blockchains, on the normal internet, we generally have unfettered access with our web browsers to view and interact with websites. In many cases, this interaction requires a server to execute code, and generally users are not asked to pay for the server costs directly. I do not pay micropayments when I post to Twitter or Instagram. I don’t keep my account loaded with funds on Facebook or even think of my interactions with the platform as transactions. Of course, as we have all been reminded by the Facebook and Cambridge Analytica debacle, nothing is truly free. Running servers that cost money means you need to pay for those servers somehow.

In the cryptocurrency world, transactions of all kinds can also be directly free, if for example, someone pays for your transactions for you, or the protocol uses a fundamentally different model than Bitcoin and Ethereum for saddling the cost of the network. Just like the web, someone must pay for the servers that run the network, but if that cost can be inserted elsewhere in the business model it may help adoption and simplify on-boarding.
<br>
<br>
#### **Private Permissioned is Usually Free**
{% include image name="7.jpeg"%}

One quick way to make transactions free is to use a permissioned ledger approach. In the supply chain space, there are many projects sprouting up that use Hyperledger Fabric to share shipment tracking as well as many other types of data: Shipment congestion history, spot delivery pricing trends, etc. Fabric ends up being a good choice because the network nodes can be supported by many different business models and those node hosts can decide how to charge for network participation. They do not need to charge every client or entity that chooses to interact with the network, so their network on-boarding process does not need to involve buying a token or paying anything. Private permissioned ledgers do not provide the same guarantees as public ledgers, but the architecture can make sense for collaboration between groups of private enterprises, such as a consortium.
<br>
<br>
#### **Public Blockchains Can Also Be Free**

Public blockchains, different than private permissioned blockchains like Hyperledger Fabric do need an incentive model for those that run nodes. This does not mean that the end user needs to be the one paying. We are starting to see other network economic models forming. For example, in the case of Ethereum there are are EIPs that allow alternate parties to cover gas costs. Some of those only make sense if a third party has incentive the transaction, so there are many caveats. We also see alternate approaches popping up, for example, EOS allows the smart contract publisher to pay network fees for user transactions, but that can create a door for spam attacks. More research is needed in the area of alternate fee structures.
<br>
<br>
#### **In Summary**

Up to this point, cryptocurrency usage has been derived from a few niche places: Philosophical alignment with decentralization, gambling, and regulatory arbitrage, to name three. Mainstream adoption, in contrast, must be derived from incentive alignment and convenience. Much can be learned from the most widely utilized payment platforms. Cryptocurrency must grow to be better, faster, cheaper, and safer than those popular payment platforms. Transaction fees are an important piece of that puzzle, and a piece yet to be solved.

<br>
This article was originally posted on Medium and [can be found here.](https://medium.com/sagewise/ethereum-transaction-fees-hamper-adoption-d1b6680ab343)