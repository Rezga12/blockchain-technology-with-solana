# Topic 02: Bitcoin History And Technical Overview

In this topic we will get into general technical details of the blockchain network taking examples from the bitcoin and it's characteristics.

Despite the fact that the course is mainly concentrated on solana development We think understanding Bitcoin mechanics is important for any blockchain developer. In addition, bitcoin may be the easiest blockchain to understand for a beginner in this field and most characteristics and core concepts will be transitioning to the different ecosystems like Solana as differences will be easier to spot and new features simpler to understand.

## Agenda

* very brief overview of history
  * who was satoshi nakamoto
  * creation of the network
  * how bitcoin gained value
  * state of the bitcoin now
* Overview of General blockchain architecture
  * What is Consensus and why is it important in decentralized application
  * Byzantine Generals' problem (Examples)
  * How bitcoin solves byzantine generals problem
  * The mining process and why there’s so much fuss about miners. What are incentives to mine
* Technologies used in bitcoin
  * In depth proof of work
  * Transactions
  * How are blocks created
  * bitcoin network participants
  * different types of nodes
  * validation and consensus
  * understanding merkle trees
* Limitations of bitcoin network
  * used only for transactions
  * Slow
  * High fees
  * Electricity consumption
  * No turing complete language to help with transactions
* Solution 1: Creation of Sidechains
  * talking about reasons
  * Benefits and Disadvantages
  * Example: The Lightning Network
* Segue to the next topic: Smart contracts and DeFi

## Overview of the resources

The main resource of this topic will be the book **Mastering Bitcoin: Programming the Open Blockchai**

This [github repository](https://github.com/bitcoinbook/bitcoinbook) covers all of the book topics.

[Bitcoin whitepaper](https://bitcoin.org/bitcoin.pdf)

demystifying merkle trees and explaining how are they used to store blocks for validation in bitcoin network: [What is a Merkle Tree?](https://decentralizedthoughts.github.io/2020-12-22-what-is-a-merkle-tree/)

Key highlights and explanation of two generals problem (aka byzantine fault tolerance problem) [What Is the Byzantine Generals Problem](https://river.com/learn/what-is-the-byzantine-generals-problem/)

The demo of how are blocks created and mined (will be goreat for demonstration purposes): https://andersbrownworth.com/blockchain/hash

The demo of creating Public / Private Keypairs (covered more in depth in next chapters). https://andersbrownworth.com/blockchain/public-private-keys/keys

videos about general bitcoin mechanics and proof of work.

* [How does bitcoin actually work](https://youtu.be/bBC-nXj3Ng4)
* [Explained proof of work in depth](https://www.youtube.com/watch?v=2hFvQhMRnc4)

Couple interesting articles about why bitcoin has value and where it comes from.

* [Debunked: What Truly Gives Bitcoin Its Value?](https://learn.bybit.com/crypto/what-gives-bitcoin-value/)
* [AN EXPLORATION OF INTRINSIC VALUE: WHAT IT IS, WHY BITCOIN DOESN’T HAVE IT, AND WHY BITCOIN DOES HAVE IT](https://bitcoinmagazine.com/culture/an-exploration-of-intrinsic-value-what-it-is-why-bitcoin-doesnt-have-it-and-why-bitcoin-does-have-it)

This topic will also contain a little introduction about side chains. taking as example bitcoin side chain [The Lightning Network](https://lightning.network/)

Bitcoin scrypt language overview: https://betterprogramming.pub/the-bitcoin-script-language-e4379908448f
[Scrypt | Bitcoin Wiki](https://en.bitcoin.it/wiki/Script)


[UTXO Model: Definition, How It Works, and Goals](https://www.investopedia.com/terms/u/utxo.asp)
https://finbold.com/guide/what-is-utxo/



