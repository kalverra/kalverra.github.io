---
title: "Cryptocurrencies For the Non-Technical"
date: 2022-03-05
draft: false
categories: ["tech-explainers"]
tags: ["cryptocurrency", "finance", "economics"]
description: A look at how crypto currencies work, why they exist, and what the future might look like for non-technical people.
summary: A look at how crypto currencies work, why they exist, and what the future might look like for non-technical people.
---

Cryptocurrencies have entered the public consciousness. Super Bowl 56 aired ads from [cryptocurrency companies](https://www.npr.org/2022/02/14/1080237873/superbowl-ads-crypto-bitcoin), and sports stadiums have been named after [similar](https://www.nbcsports.com/washington/nationals/nationals-accept-cryptocurrency-ballpark-early-2023-season) [organizations](https://en.wikipedia.org/wiki/Crypto.com_Arena). Local and national news outlets' coverage of these events &mdash; laden with technical jargon that is often laughably misused &mdash; often makes audiences turn to their nearest tech-literate acquaintance and ask, "what are those exactly?". As a member of the the tech-literate, I'm consistently disappointed with my answer to this question. It's often half-assed and satisfies neither me nor my less-than-captive audience. So here's my attempt at a high-quality answer.

**Disclaimer**: I've been working seriously in the cryptocurrency space for a little over a year. That's a relatively long time given how new this tech is, but I'm not an expert. Also, while I work on a cryptocurrency project, all opinions are solely my own, and I'm sure my co-workers would vehemently argue against at least a few of them.

## How They Work

You don't need to know how cryptocurrencies work to use them; just like you can use your credit card without intimate knowledge of how the banking system works. As the technology matures, it will become simpler for the layperson to use and understand. It's for this reason that I find most cryptocurrency explanations to a general audience lean far too technical. That's because a lot of the people in this space are tech nerds, and the tech behind cryptocurrencies is revolutionary and complex, so tech nerds believe that's the part everyone is interested about. In reality, such explanations quickly devolve into acronyms and esoteric computer terms that bore audiences to sleep. So I'll keep the explanation on *how* this tech works brief: Math[^1]. Primarily a study of math and computer science called [cryptography](https://youtu.be/jhXCTbFnK8o), thus the name *crypto-currencies* (often abbreviated to *crypto*).

An important aspect to understand is that cryptocurrencies live on a [blockchain](https://en.wikipedia.org/wiki/Blockchain). A blockchain is... well a chain of blocks, each block containing a record of transactions between people. New transactions get put into these blocks and added on to the chain. There is no single, capital B blockchain, and multiple currencies can live on a single chain. Most people have heard of[^2] the O.G. chain and currency, [Bitcoin](https://bitcoin.org/en/), but there are hundreds more blockchains and millions more currencies now. Many in the crypto community actually consider Bitcoin a bit of a relic[^3], and the blockchain technology most people are working on now is [Ethereum](https://ethereum.org/en/).

## Why They're Important

Cryptocurrencies have some unique traits that distinguish them from normal currencies, primarily that they are decentralized. Unlike typical currencies, there is no central entity that controls the currency or its operation[^4]. No government or bank can decide to print more or less of the currency, and if you want to change how the currency is issued or operates, you usually need to propose such changes for a vote by the community. And if a government wants to shut down or ban cryptocurrencies, it's near impossible, as the people operating the blockchain are scattered around the world, and hard to find anyway.

The blockchain world is also predicated on the idea of trustless technologies. You can mathematically verify everything, read the code of companies you interact with, and [see every program and transaction](https://etherscan.io/) that happens on the blockchain[^5]. You may say "I don't know the math, I'm just trusting you that's the case!". Sure, but you can learn the math, or go to another person that knows the math, or use a program that confirms it. Whereas no matter how long I ask Goldman Sachs to show me their books, they keep blowing me off, telling me disrespectful things like "who are you?" and "please stop drinking liquor and yelling at our office"[^6]. On a blockchain you can see every transaction your bank or government or anyone has ever made, all while drinking liquor and yelling at your cellphone instead of a big office building.

It's not just transactions that happen on this public chain, but also programs. You can write a program (called a [smart contract](https://ethereum.org/en/developers/docs/smart-contracts/)) and put it on the blockchain as well. From there, anyone in the world can read the code of the program and execute it if they so choose. This enables entire companies and governments to operate on the blockchain, putting their products and services out for anyone on the chain to use.

This is a fundamental shift in not only how currencies usually work, but also how technology usually works[^7]. Any time something like that happens, the tech and finance nerds emerge from their basements to tell anyone and everyone about it. It's especially exciting because the banking industry has long been behind the times when it comes to technical innovation, and this crypto business has thrown a giant wrench in the normal state of affairs for them.

What if you trust your government or bank to make good monetary decisions? Well, I'd encourage you to be a [bit less trusting](https://foreignpolicy.com/2021/01/28/report-transparency-international-corruption-worst-decade-united-states/), but also to realize that many people don't have that option. Cryptocurrencies and smart contracts enable people in developing countries &mdash; who typically have low trust in their country's government and businesses &mdash; to use services like [crop insurance](https://www.coindesk.com/business/2021/12/14/accuweather-taps-chainlink-to-explore-crop-insurance-and-more/) without fear of being scammed or having the terms of their contracts change
on a whim. These benefits will start to become more and more attractive in more developed countries as businesses and governments see that they can reduce risks with them.

What if you **want** your transactions to be private? Well, you're in luck, everything on blockchains is pseudonymous. Transactions don't look like `Adam paid Meg $5`. [Here's a recent transaction](https://etherscan.io/tx/0x01e2784e34ff05d1cf01a8d8dfe6fddbdce2e1495f3056973d8f81c2b5e72dfa) on Ethereum:

```txt
0xa15a3dda54758f447ce55873d46103cc860ca0f9 
paid 
0xa57976422edafff7d3545a6b58150afdd9e59faf 
0.021 Ether ($63.50)
```

`0xa15a3dda54758f447ce55873d46103cc860ca0f9` is an address, and that is how you send money around in a blockchain, by sending from your address to others. They function a bit like usernames on sites like Reddit or Twitter. You can make it your real name if you like, or just name yourself `420cat420` and leave it at that.

----

**Here's primarily where we step into "Adam's Personal Opinion Zone". Ye be warned.**

----

## What They Could Become

Most people[^8] working in the space see cryptocurrencies as a turning point in tech and society, much like the internet was. In fact, many call the world of blockchains and cryptocurrencies "Web 3.0".

The counterpoint I most hear is that crypto is a fad, or a solution looking for a problem.

![Yeah? Well, you know, that's just like, your opinion, man](https://i.imgur.com/sNebp1W.gif)

At a minimum, cryptocurrencies have, and will, further disrupt how transactions work. There's a massive infrastructure dedicated to moving money around that is antiquated, slow, and only gets more complicated when you cross national borders. These are all classic indicators that technology can optimize and replace the current system. Cryptocurrencies do things &mdash; like confirm payments &mdash; in seconds that take traditional banking and finance days.

People sometimes scoff at cryptocurrencies as a stupid tech nerd thing that isn't useful to them. To that, I present to you a clip of Bill Gates trying to explain the internet to David Letterman in 1995.

{{< youtube gipL_CEw-fk >}}

Doesn't sound too revolutionary does it? Bill Gates, the king of computer nerds and one of the greatest businessmen in the world, was only able to think of radio and email as the future of the internet. Back then it was normal to be skeptical of this nerdy internet thing, but if you ask "what is that internet thing anyway?" you're typically met with looks of confusion or pity. Back then it was a niche technology that only nerds got excited about, and now the internet dominates our modern society.

But there's a problem with the internet today: ads. They are the reason Google makes $257.6 billion a year, and they are the reason why tech companies like Google collect a [frightening amount of information](https://youtu.be/wqn3gR1WTcA) about you. Targeting ads based on your personal data is a lucrative business, and a precursor to some dystopian [1984](https://www.goodreads.com/book/show/5470.1984) shit. You remember how terrifying that book was? Or how dark the SparkNotes summary sounded when you were cramming before that 10th grade English class? Cryptocurrencies and blockchains enable different profit models, ones that don't depend on collecting your personal data and selling it to the highest bidder.

Humans are notoriously bad at predicting the future, so only time will tell the truth. But some exciting areas that cryptocurrencies could revolutionize include [voting](https://vitalik.ca/general/2021/05/25/voting2.html), [cities](https://vitalik.ca/general/2021/10/31/cities.html), [insurance](https://blog.chain.link/blockchain-insurance/), banks, and modern internet infrastructure.

## FAQ

### How Can I Use Them Right Now?

I suspect things will drastically change in the next 10 or 20 years, but for now the use of these technologies is primarily regulated to early-adopters and builders that are deep into technology or finance. Things like currency exchanges, loans, gambling, and video games[^9] dominate the current crypto world, and most of them require some detailed tech knowledge to use correctly. There's not much, that I know of, for the casual observer to do with the crypto world, *right now*.

### NFTs?

I think current iterations are kinda dumb.

For those uninitiated to the latest tech news cycle, blockchain technology enables owning not only currency, but damn near anything. Currency is [fungible](https://www.investopedia.com/terms/f/fungibility.asp#:~:text=Key%20Takeaways-,Fungibility%20is%20the%20ability%20of%20a%20good%20or%20asset%20to,houses%2C%20are%20non%2Dfungible.), meaning that a one dollar bill isn't worth more than another one dollar bill. As far as the typical consumer is concerned, they're identical in value and usage. NFTs are **N**on-**F**ungible **T**okens, meaning they're unique.

All this is to say that you can use blockchain tech to show your ownership of unique objects like [art](https://www.theverge.com/22310188/nft-explainer-what-is-blockchain-crypto-art-faq). Frankly, the art market [could use some disruption](https://freakonomics.com/podcast/a-fascinating-sexy-intellectually-compelling-unregulated-global-market/), but what troubles me is how the crypto community tries to proselytize art NFTs as the big crypto thing. NFTs have some interesting uses like replacing typical land and house deeds, but showing people a picture of a cruddy, pixilated avatar and saying "see, the future!" is, at the least, lacking in creativity. It seems to me like trying to convince someone that Baseball is a cool sport to watch, and then showing them all you baseball trading cards to convince them.

### Environmental Impact?

It's not great. The process most blockchains use to operate is a [consensus mechanism](https://ethereum.org/en/developers/docs/consensus-mechanisms/) called Proof-of-Work, which entails people running very expensive and energy inefficient programs[^10] on their computers. But, there's hope that this will change soon. Proof-of-Stake is a method that blockchains can use that consumes 99% less electricity, and most new chains use it. Others like Ethereum are [actively working](https://www.technologyreview.com/2022/03/04/1046636/ethereum-blockchain-proof-of-stake/#:~:text=Of%20course%2C%20Ethereum's%20move%20to,such%20a%20model%20is%20complex.) to switch to this system.

### Money Laundering?

It's harder than you think. The blockchain is completely open, and a permanent record of every transaction ever made. Money launderers aren't huge fans of having all their transactions publicly available by any FBI agent or teenager who cares to take a look. That said, blockchains are [pseudonymous](https://www.thefreedictionary.com/pseudononymous), meaning that you can easily hide your real-life identity on the blockchain, but there's not a lot of options for turning your crypto currency into hard cash without alerting the government.

### Hacks and Scams?

Scams are unfortunately common in the crypto world right now. This is a symptom of the technology being new, and people not really knowing how things work. Most of them essentially boil down to "we're the password police and need to ask you some questions". Hopefully improving the user experience and knowledge will improve things.

Hacks in the crypto world are currently getting a lot of publicity thanks to the massive amounts of money that are being stolen. This is another symptom of new technology, meaning that people are still figuring out the pitfalls and security loopholes. Blockchain tech also has the unique property of being totally open, meaning that a hacker can often see all the code of the thing they're trying to hack, information that most hackers would kill for. It also means that people know when these hacks happen immediately, as all these things are public. A lot of companies, when hacked, will do their best to cover it up. Cryptocurrency projects lack that privilege.

### Taxes?

It's... complicated. Most tax lawyers don't know what's going on most of the time, and legislation is changing all the time. Suffice to say that any time you turn cryptocurrency into real cash, the government knows, and will ask for their cut.

### Dogecoin and Elon Musk?

It's also complicated, but less so. [Dogecoin](https://en.wikipedia.org/wiki/Dogecoin) is a cryptocurrency that was created as a sort of in-joke among crypto people. It doesn't serve any purpose except as a weird techie joke, and it hit mainstream recognition when Elon Musk [tweeted](https://abcnews.go.com/Business/dogecoin-rallies-elon-musk-tweet/story?id=82265024) about it. People got it in their minds that since tech genius Elon Musk was talking about Dogecoin, it must be a sound investment. It's not. He was either joking, or [is wrong](https://vitalik.ca/general/2021/05/23/scaling.html). There have been recent attempts to actually revive the project and turn it into something worthwhile, we'll see where that goes.

### Should I Invest / What Should I Invest In?

I can't tell you / I can't tell you. I **can** tell you that you should probably should invest in something, but for the majority of people, cryptocurrencies are probably not that something[^11]. The crypto markets are uniquely risky, and most currencies aren't really designed to be investment vehicles anyway. There are thousands of YouTubers, bloggers, and podcasters that will promise untold crypto riches if you listen to their sure-thing advice where they show some fancy charts and make insane predictions. They're lying, either to you or themselves.

There's lots of speculation on cryptocurrency prices now, and currently not a whole lot of mainstream functionality exists, leading to more speculation of a possible [dot-com style bubble](https://en.wikipedia.org/wiki/Dot-com_bubble). Suffice to say that if you're reading this post to explain cryptocurrencies to a beginner, there are a lot more steps to take on educating yourself before you try to invest in these projects.

### I'm interested, Where Can I Learn More?

Chainlink has [set up a hub](https://www.smartcontracthub.dev/) to help people learn more about the tech. Chainlink Labs's CEO, [Sergey Nazarov](https://twitter.com/sergeynazarov?lang=en), did a [long interview](https://youtu.be/TPXTmVdlyoc) last year on these topics.

[Vitalik Buterin](https://en.wikipedia.org/wiki/Vitalik_Buterin), the key figure behind Ethereum, does a lot of outreach. He has done [some](https://youtu.be/3x1b_S6Qp2Q) [interviews](https://youtu.be/XW0QZmtbjvs) that non-techies should find approachable. He also does some deep technical writing on [his website](https://vitalik.ca/).

Gary Gensler, the current head of the SEC, taught a course at MIT on the finance side of blockchains and cryptocurrency that is available for free [on YouTube](https://www.youtube.com/playlist?list=PLUl4u3cNGP63UUkfL0onkxF6MYgVa04Fn). It's long, but invaluable resource.

### I'm Interested, How Can I Work On This Stuff?

You're in luck, demand is high! Chainlink [is hiring](https://chainlinklabs.com/careers) for nearly everything right now, and there's plenty of others [looking for](https://cryptocurrencyjobs.co/) eager employees.

[^1]: If you'd actually like to learn more deeply about the technology behind cryptocurrencies, check out [this excellent video](https://youtu.be/bBC-nXj3Ng4) that doesn't require any background in math or computer science.

[^2]: Lots of people haven't heard of [Satoshi Nakamoto](https://en.wikipedia.org/wiki/Satoshi_Nakamoto) though, the creator of the coin. Their story is an interesting one, because no one knows who they are. The name is a pseudonym, and there's some guesses, but no definitive reveal as to who this person actually is (they also stopped posting in 2010). As such, some people in the crypto community elect to do something similar, and are only identified by their online profile names.

[^3]: Those who think Bitcoin is **not** a relic often like to write mean things on the internet about people who say otherwise. It's a whole culture war I won't get into.

[^4]: There are some rare situations where this isn't the case, like when a company has their own private implementation, or when a scammer is trying to swindle you out of your money.

[^5]: [Monero](https://github.com/monero-project/monero) is a notable exception to this rule, but it's rather fringe. It's a cryptocurrency project that hides account balances and transactions.

[^6]: Those fascist pigs

[^7]: Not the drunkenly yelling at your cell phone though, that mostly stays the same.

[^8]: It was far more common in the early days for anarchists and libertarians to assert that the invention of Bitcoin and similar currencies would be the turning point for revolution, that the world would now operate without governments entirely. The crypto community still skews libertarian by its nature, but most have disposed of the whole "completely dismantle all governments" idea. Most focus on just partially dismantling governments and mostly dismantling banks.

[^9]: As an avid gamer, these are pretty lame. Personally I don't think video games and cryptocurrencies will mix very well in the future, but I guess we'll see.

[^10]: This process often uses a specialized piece of computer hardware called a GPU, or graphics card. They're typically used by people who do a lot of visual work on their computers like animations and 3D models. They're also used by people like me who play a lot of video games on their computer. So I'm very eager for Proof-of-Stake to happen for not only environmental reasons, but also because people keep buying all the graphics cards and I cannot get one to play games with!

[^11]: If you'd like to learn about investing strategies and how markets work, [these](https://www.goodreads.com/book/show/40242274-a-random-walk-down-wall-street) [books](https://www.goodreads.com/book/show/106835.The_Intelligent_Investor) [are](https://www.goodreads.com/book/show/38315.Fooled_by_Randomness) [great](https://www.goodreads.com/book/show/381355.The_Bogleheads_Guide_to_Investing). Here's a [cheat-sheet](https://www.reddit.com/r/personalfinance/wiki/investing) if you're not quite that *invested* in the topic.
