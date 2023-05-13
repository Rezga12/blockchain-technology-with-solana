# Topic 05: Ethereum Technical overview and architectural components

We already discussed Ethereum history and purpose of it's creation in topic 03. Here we will be talking about it's architectural Componnents, how these components interact with each other to constitute all the features and benefits of this blockchain. We will also have a look at it's main limitations and all the 3rd party technologies made created to get through the boundaries of these limitations. This topic will be somewhat a high level overview of Ethereum features and components, practical examples will be incorporated in the next few topics.

## Agenda

* Introduction
  * Main limitation of the Bitcoin network: no room for building applications
    * _Script_ language
  * Reviewing of some attempts of solving bitcoins limitations before Ethereum
    * Colored coins
    * Bitcoin cash
    * Namecoin
    * The lightning network
  * Code is law: the importance of smart contracts
* Overviewing Core architectural Components
* Ethereums anti-denial of service model: **The Gas**
  * How gas fees work
  * How is gas amount calculated per transaction
  * What takes up gas
  * How are gas prices Adgusted per each confirmed block
  * How gas fees are distributed
  * London upgrade and **EIP-1559**
* Ethereum State Transition Function
  * Overviewing transaction structure and fields
  * messages ("transactions" between contracts)
  * The execution flow
  * What happens if the transaction(or message) fails to complete
* EVM _(Ethereum Virtual Machine)_ and Code Execution
  * From Ledger to state machine
  * How The Distributed state machine works&#x20;
  * EVM is what defines the rules for computing next valid state
  * Instructions for EVM's stack based model
  * Types of data storages
    * stack
    * memory
    * storage
  * Computational state tuple: _(block\_state, transaction, message, code, memory, stack, pc, gas)_
  * _EVM implementations, why there's so many of tham and why doesn't Ethereum team has it's own one_
    * [Geth](https://geth.ethereum.org/) (Go)
    * [_Nethermind_](https://nethermind.io/) _(.NET)_
    * [_Besu_](https://besu.hyperledger.org/en/stable/) _(Java)_
    * [_Erigon_](https://github.com/ledgerwatch/erigon) _(Go)_
* Blockchain and Mining Process
  * Underline all the similarities with bitcoin _(There's quite a lot of them)_
    * POW mining _(before the Ethereum 2.0)_
    * Mem Pools
    * Block structure (With slight differences from bitcoin)
    * Tx Validations using merkle trees _(just as in case of bitcoin)_
  * Differences with Bitcoin:
    * Block structure and storage of the current state
  * Where and When the contract code is executed
* &#x20;**Ethereum 2.0 and The Merge**
  * The next upgrade for ethereum ecosystem
    * improved scalability, accessibility and transaction throughput
    * introduced proof of stake instead of proof of work
  * What is proof of stake
    * Benefits and disadvantages compared to proof of work
    * Proof of stake validator coordination
    * how a transaction gets executed in ethereum POS
    * proof of stake and security
  * What was **The Beacon Chain** and what did it do
    * The introduction of staking
  * Revision of **the forks** in blockchain
  * **The Merge** _(Paris Upgrade)_
    * How the beacon chain merged with the main chain
    * Describing the process

## Overview Of The Sources

Although bitcoin doesn't have Conventional smart contracts, it has a language names **Script** in it's transactions. \
[What is Bitcoin Script](<../../Lecture Main Topics/Topic 02 Bitcoin History And Technical Overview.md>) - the article about the language and what is it used for. \
[Script | Bitcoin Wiki](https://en.bitcoin.it/wiki/Script) - from bitcoin wikipedia page\
We will be talking about Why Turing-completeness matters and what are the limitation of bitcoin in terms of smart contracts.\


The attempt to create Tokens on bitcoin network: [Bitcoin _colored coins_ and how they work](https://academy.bit2me.com/en/what-is-a-colored-coin/)\
[The brief history of colored coins and why they didn't became a thing](https://cryptoadventure.com/a-brief-history-of-colored-coins-what-made-them-special/) - Also an interesting read\
[The Lightning Network](https://lightning.network/) was also an attempt to coup with the bitcoin't limitations, introducing more scallability and low transaction costs. It was first ever layer 2 blockchain.



We talked about bitcoins limitation and the attempts to solve them, now we will talk about Ethereum:

[Ethereum - Architectural Components](https://cointelegraph.com/learn/architectural-components-of-the-ethereum-blockchain-what-are-they) - Brief article about main etherium features and componnents.\
[Ethereum whitepaper ](https://ethereum.org/en/whitepaper/)- it covers almost all the main topics to talk about when discussing it's architecture. Also a really interesting read.

[Gas and Fees](https://ethereum.org/en/developers/docs/gas/) - From Ethereum Docs\
[Gas Fees Tracker](https://etherscan.io/gastracker) - Just to have a look what it looks like in real world\
[EIP-1559 - How Will it change Ethereum.](https://consensys.net/blog/quorum/what-is-eip-1559-how-will-it-change-ethereum/)\
[youtube video about EIP-1559](https://www.youtube.com/watch?v=MGemhK9t44Q) from finematics.

[Units of gas for every EVM instruction](https://ethereum.org/en/developers/docs/evm/opcodes/) - The page is for just demonstrating purposes. units of gas the transaction will consume are calculated by each EVM stack instruction when executing a smart contract.

[Ethereum Evm Illustrated](https://takenobu-hs.github.io/downloads/ethereum\_evm\_illustrated.pdf) - How evm works internally explained with illustrations.\
[Etherium Virtual Machine](https://ethereum.org/en/developers/docs/evm/) - From Ethereum docs page.\
List of [ethereum execution clients](https://ethereum.org/en/developers/docs/nodes-and-clients/#execution-clients). This much disparity in client implementation shows high degree of decentralization. etherium team doesn't even have their own client implementation. (altho[ geth takes 80%](https://www.ethernodes.org/) of all deployed clients on mainnet)

The List of all [Ethereum Updates historically](https://ethereum.org/en/history/#2023). some of them are only the pushing of [difficulty bomb](https://ethereum.org/en/glossary/#difficulty-bomb), but by going through all the updates you will learn much more about the history of the ecosystem\
An article about [the beacon chain](https://ethereum.org/en/roadmap/beacon-chain/): helper chain that introduced proof of stake on ethereum network.\
Comparision between POW and POS: [https://blockgeeks.com/guides/proof-of-work-vs-proof-of-stake/](https://blockgeeks.com/guides/proof-of-work-vs-proof-of-stake/)\
The Merge (Paris Upgrade) - [Finematics video explanation](https://www.youtube.com/watch?v=EEuPmA8w0Kc)\
Article from Ethereum.org: [https://ethereum.org/en/roadmap/merge/](https://ethereum.org/en/roadmap/merge/). this resources explain how the merge was operated without any major forks taking place.
