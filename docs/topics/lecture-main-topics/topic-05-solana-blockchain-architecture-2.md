# Topic 05: Solana Blockchain Architecture

This topic serves as a form of introduction of solana blockchain. Here we will underline it's key features and benefits. As the audience already should have general grasp of how things work in a blockchain ecosystem some topics will be easier to read and easier to understand. The accents will be held mostly on Solana architecture and Will have mostly educational approach than hands on tutorials.

## Agenda

* Introduction
  * A brief history of Solana
  * Key features and advantages compared to other blockchains
  * Overview Of The solana Ecosystem
* Architecture
  * Network Design
  * Proof Of History
  * Proof Of Stake
  * Transaction Processing and pipelining
  * Block Propagation Algorithm
  * How Solana solves Two Generals Problem (TowerBft)

## Overview Of Sources

[Entry level Overview of solana](https://2501babe.github.io/posts/solana101.html)

[What is Solana? SOL Explained with Animations](https://www.youtube.com/watch?v=1jzROE6EhxM)

Explaining Solanas key innovations for non developers: [Solana's Innovations - a jargon-free explanation](https://learn.figment.io/tutorials/explaining-solana-for-beginners)

Articles About Solanas 8 Key innovations:

* [Proof Of History:](https://medium.com/solana-labs/proof-of-history-a-clock-for-blockchain-cf47a61a9274) A Clock for Blockchain
* [Tower BFT:](https://medium.com/solana-labs/tower-bft-solanas-high-performance-implementation-of-pbft-464725911e79): Solana’s consensus algorithm implementation
* [GulfStream:](https://medium.com/solana-labs/gulf-stream-solanas-mempool-less-transaction-forwarding-protocol-d342e72186ad) Solana's mempool-less Transaction forwarding Protocol
* [Sealevel:](topic-05-solana-blockchain-architecture-2.md) Parallel smart contract tuntime
* [Pipelining:](https://medium.com/solana-labs/pipelining-in-solana-the-transaction-processing-unit-2bb01dbd2d8f) The Transaction processing unit
* [Turbine:](https://medium.com/solana-labs/turbine-solanas-block-propagation-protocol-solves-the-scalability-trilemma-2ddba46a51db) A block propagation protocol
* [Cloudbreak:](https://medium.com/solana-labs/cloudbreak-solanas-horizontally-scaled-state-architecture-9a86679dcbb1) Horizontally scaled account database
* [Archivers:](https://docs.solana.com/proposals/ledger-replication-to-implement) Solana's distributed ledger technology, ledger replication

There's no need to go into details of all those features, but would be benefitial mentioning them Also there are several good articles about transaction lifecycle on solana and why transactions are getting skipped:

* [Solana Validator 101: Transaction Processing](https://jito-labs.medium.com/solana-validator-101-transaction-processing-90bcdc271143)
* [Solana Cookbook: Retrying Transactions](https://solanacookbook.com/guides/retrying-transactions.html#facts)

Also this video covers and explain a lot of implementation details and how are all things connected int the network: [Whiteboard Series with NEAR | Ep: 2 Anatoly Yakovenko from Solana](https://www.youtube.com/watch?v=rKGhbC6Uync) Here's [Conspects](https://github.com/lsmod/proof-of-history-explained#ok-i-get-proof-of-history-whats-the-point) for the video
