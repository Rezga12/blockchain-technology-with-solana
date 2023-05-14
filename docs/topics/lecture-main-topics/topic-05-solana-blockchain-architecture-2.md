# Topic 08: Concept of Oracles and Layer 2 protocols

In previous section we talked about limitations of smart contracts. The oracles - third party trusted entities to aid enhancement of smart contract functionality were introduced for that matter.We will be talking about the most well known chain of oracles: **Chainlink.** also we will discuss the concept of layer 2 protocols _(through not in great detail)_ and discuss what are their benefits and how are they used. The most relevant example will be **Polygon** blockchain.

## Agenda

* The concept of oracles
  * The problems with traditional smart contracts
    * how to determine current gas price
    * determine current USD value of Ethereum
    * Determine the state of the weather
    * Flip a Coin (Heads / Tails)
    * make an API call to the external resource
  * How oracles work
  * Common use cases and examples of oracles
* **Chainlink**
  * The oracle problem and how chainlink solves it
    * Chainlink protocol: the standard for oracle networks
  * LINK token and how it is utilized
  * Chainlink features:
    * Data feeds
    * Chainlink functions
    * Automate Contracts
    * Verifiable Random functions
    * External API calls
* Examples of using Data Feeds
  * Example 1: assert function on sent value in USD
    * how to use Chainlink ETH/USD Price feed in a smart contract
  * Example 2: writing simple coin flip view function in a smart contract
    * how to use Chainlink VRFs
* Layer 2 protocols
  * The problems with ethereum
    * high transaction fees / gas price
    * low scallability
  * Polygon: Layer 2 for ethereum
    * how polygon functions
    * what are **rollups**

## Overview Of Sources

youtube videos:\
[What are Oracles in Crypto? (Animated) - Whiteboard Crypto](https://www.youtube.com/watch?v=uycQ7ReSt\_c)\
[What is a Blockchain Oracle? | Chainlink Engineering Tutorials](https://www.youtube.com/watch?v=ZJfkNzyO7-U)

[What is a blockchain oracle | Medium article](https://betterprogramming.pub/what-is-a-blockchain-oracle-f5ccab8dbd72)

[https://supraoracles.com/academy/what-are-oracles/](https://supraoracles.com/academy/what-are-oracles/) - a good article about different types of oracles and their use cases. also a good related articles section.

[Chainlink exploits lead to ETH losses—again](https://coingeek.com/chainlink-exploits-lead-to-eth-losses-again/) - a small article about what might happen if you trust too much in oracles.

how chainlink data feeds work: [Chainlink Data Feeds](https://docs.chain.link/data-feeds)\
[using data feeds](https://docs.chain.link/data-feeds/using-data-feeds)

[Introduction to Chainlink VRF](https://docs.chain.link/vrf/v2/introduction) - we will discuss VRFs and other chainlink functionality just in the sake of demonstration. we will not be going in much more detail. if students have interest in learning about them we will be happy to provide additional resources and code samples.

\
[Polygon (MATIC): The Swiss Army Knife of Ethereum Scaling](https://www.gemini.com/cryptopedia/polygon-crypto-matic-network-dapps-erc20-token) - briefly about polygon.
