# Layered Bitcoin

> If something is valuable enough, monumental efforts will be made towards rectifying its flaws.

The exciting stuff in Bitcoin happens in layers.

Because the base protocol is kept intentionally stable, it acts as bedrock for other developers to build upon.

It's important to acknowledge that the Bitcoin protocol is more than just what's contained within [Bitcoin Core](https://github.com/bitcoin/bitcoin), and that code on its own is unable to efficiently solve for all that it could, and wouldn't change much at all if it weren't for an entire industry working very hard towards finding a use for Bitcoin in every little niche.

In many ways, Bitcoin automates banking. It does this without recreating a system based on debt or trust. And as current systems are showing signs of failure, censorship, fragmentation, and hyperinflation, it is imperative that resources are put towards rebuilding the world's financial systems upon firmer foundations.

For this, an entire ecosystem is needed. Wallets and layers, clients and indexes, software nodes and hardware nodes. All these are needed to fulfill the promise of Bitcoinization: A world in which the corrupt elites can no longer exploit and control through monetary manipulation.

A Bitcoin layer can be defined as an open protocol that uses the Bitcoin timechain or the BTC currency, as denominated in either ₿itcoins or ṩatoshis, to extend the capabilities of the protocol below it.

An open protocol can be defined as open source software that can be either embedded or run independently of its developers, and thus is truly decentralized.

Scaling is also good for furthering the cause of adoption; layers often implicitly come with improvements in scale, cost, privacy, and functionality.

Scalability comes from the capability to delay settlement onto the layer below. This also goes hand-in-hand with cost savings, and in some cases, enables entirely new avenues of functionality, if not entire industries. For example, Lightning Service Providers, Lightning Liquidity Providers, and Value-4-Value are all burgeoning industries in their own right.

The term timechain is used instead of blockchain or cryptocurrency, since these words were not used by Satoshi in the original whitepaper, whereas the word "timechain" was used in original distributions of the Bitcoin node. This is also useful because many Bitcoin imitators will attempt sell themselves as "Better than Bitcoin" or "Bitcoin alternatives" that use the same or similar technology that Bitcoin uses, and thus, is at least as trustworthy and decentralized as Bitcoin is. This is what's known as an "affinity scam", since the identity of the founders of those scams is known, they will always suffer from weaknesses in either security or market manipulation that Bitcoin avoids, because the identity of Satoshi Nakamoto has never been proven. This is why Bitcoin is different, and anything else that introduces its own form of money is actually a rugpull or inflationary affinity scam, no matter how sincere its founders might appear.

Imitators did serve a purpose in many ways, in showing either what not to do, or what can be done, just not in that way. They can prove there's demand, and anything with merit will ultimately be built upon Bitcoin and only Bitcoin.

## Axioms

Axioms of a Bitcoiner, short and easy to remember

1. Everything is good for Bitcoin (because attacks harden the protocol)
2. Bitcoin is good for everything (just not always on its own)
3. Bitcoin is for everyone (including people you don't like, doing things you don't care for)
4. Bitcoin does not need you (it will survive if you do not)
5. Bitcoin isn't perfect (and it doesn't need to be to replace all money)

Layers help with point 3, because not everyone is going to want to learn about self-custody.

## Layers by Purpose

Often, layers are enumerated, but it's also helpful to conceptualize Bitcoin layer protocols by categorizing them by purpose.

### Accounts Layer

Electrum Server was one of the first accounts indexes built for Bitcoin. It has many different implementations in different languages, some of which are compared in [these](https://blog.keys.casa/electrum-server-performance-report/) two [articles](https://blog.keys.casa/electrum-server-performance-report-2022/).

LNBits and LNDHubX an accounts layer for Lightning. LNBits extends the capabilities of a Lightning node in many ways, supporting streaming sats and value-for-value apps. LNDHubX is a more minimal implementation of self-hosted Lightning accounts. Both offer [LNURL](https://github.com/lnurl/awesome-lnurl) support, which can be used for either making or receiving payements.

### Payments Layer

Lightning and Eltoo are both very good payments layers. Eltoo requires an L1 change which will require a soft fork,

A note about soft forks: Although softer and less controversial, a fork is a fork, and any fork that fails to gain adoption is by definition a hard fork. Changes to the the protocol must be kept very minimal and uncontroversial, otherwise externalities that might be perceived as negative may result much later on.

[CLN](https://github.com/ElementsProject/lightning) and [LND](https://github.com/lightningnetwork/lnd) are the two most popular implementations of Lightning Network Protocol, but [LDK](https://github.com/lightningdevkit) and [LNP](https://www.lnp-bp.org) are also growing in maturity and adoption while experimenting with new technologies like async payments (useful for browsers and mobile devices), PTLCs (which improves receiver privacy) and alternative units of account (tokens). LND has in some ways more commumnity support, with CLN a close second while offering more performance and better security. LDK is very flexible and is more for developers to build their own clients and nodes.

### Banking Layer

Accounts and banking are similar, but not the same. In the era of Free Banking, banks issued their own notes, and formed networks with other banks. Nowadays software has replaced most of these old jobs and institutions, often with a democratizing effect, and now free banking can be done in protocol form now, too. These are called [Chaumian Mints](). Users will get a means to authenticate, similar to how their old banks used emails and passwords, and will deposit their money in exchange for banknotes. There are at least two such protocols in existence, [Fedimint] was an earlier implementation and [Cashu] is one that's growing in popularity. Sats will be deposited, and are used for settlement outside of banks and between banks. It's worth noting, these make compromises in self-custody in order to develop better solutions for ease-of-use and fee reduction, and it's still better than the existing system since it's in a protocol that anyone can run, which helps resist market tendencies towards centralization and monopolization.

### Management Layer

A management layer can assist in managing the software needed to run other layered protocols. Examples of such are the [Start9 Embassy](https://start9labs.com/), [Umbrel](https://umbrel.com), and . There are also good clients, like [FullyNoded](https://fullynoded.app) and [Zeus](https://zeusln.app).

### Privacy Layer

Layers intrinsically increase privacy by keeping activity secured while not necessarily visible on-chain. There are also protocols designed specifically for privacy, such as [JoinMarket](https://github.com/JoinMarket-Org/joinmarket-clientserver) and [Payjoin](https://payjoin.org).

### Contracts Layer

TODO: Contracts Layers

### Market Layer

TODO: Market Layers

### Social Layer
TODO: Social Layers

### Storage Layer
TODO: Storage Layers

## Layers by Height

After the Block Size Wars, it was decided to keep blocks small, for many, many reasons which would often be vindicated in hindsight by looking at what the imitators chose to do instead. Out of this development came a "layered money" narrative, and we have the following two layers:

- L1: Bitcoin
- L2: Lightning

This is simple enough. But going beyond that, one thing that complicates this narrative are the inevitable questions...

Is a chain of any kind an L1? What layer are sidechains or statechains or spacechains or chains using validity proofs?

What of alternative L2 payments networks like Eltoo that rely on [features that don't yet exist](https://bips.dev/118/)?

RGB tokens make use of both L1 and L2, so it's an L3 right? But tokens with a supply of 1 and precision of 0 have no liqudity, and so cannot integrate into payments networks. So, perhaps a rule can be made that a layer above can be considered to settle upon any of the layers below.

TODO: L3
