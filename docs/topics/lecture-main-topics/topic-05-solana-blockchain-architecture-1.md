# Topic 07: Solidity and advanced smart contract concepts (via examples)

There are several languages to develop smart contracts on Ethereum, but we will be mostly focusing on Solidity as it's the most accepted one. In this section we will look at some solidity examples and go into more detail about all the stuff that might be important during smart contract development. we will also talk about the limitations of smart contracts and why they have no contact with outside world.

## Agenda

* Solidity overview
  * different compiler versions and choosing between them `pragma` keyword&#x20;
  * Declare / Create contract
  * constructor
  * storage variables
  * constants and readonly variables
  * primitive types
    * signed and unsigned integers with different sizes
    * boolean
    * bytes and strings
  * Math operations
  * Structs
  * Special `address` type
  * arrays
  * mappings
  * functions
    * declaring functions
    * view functions
    * pure functions
    * function visibility
      * public
      * private
      * internal
      * external
  * sending ETH value with message
    * payable functions
    * `msg` special variable
  * more advanced concepts
    * storage vs memory
    * Events
    * custom modifiers
    * `keccak256` build-in hash function
    * type casting
* Common code examples using solidity
  * Storage contract
  * simple fund-me contract
  * receiving and sending ETH
    * `receive` special function
    * `fallback` special function
* Limitations of EVM smart contracts
  * no contact with outside world
  * No way to determine current price
  * no way to get random value
  * API calls are impossible
  * segue to next topic: oracles and layer2 blockchains

## Overview Of Sources

[Solidity fundamental concepts | Medium article](https://coinsbench.com/solidity-fundamental-concepts-e549f175c613)

[Introduction to smart contracts | Solidity documentation](https://docs.soliditylang.org/en/v0.8.20/introduction-to-smart-contracts.html)

[https://solidity-by-example.org/](https://solidity-by-example.org/) - The collection of common code snippets With explanations. written in solidity.\
