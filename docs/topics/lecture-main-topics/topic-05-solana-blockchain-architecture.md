# Topic 06: Smart Contract Structure (via EVM)

This topic will dive deeper into EVM and smart contract development. The main purpose of this section will be to make several things as clear as possible: At what stage are smart contracts executed, How does EVM handle the execution, how are smart contracts deployed and stored on a blockchain and how is decentralization applied in all of this. We will also talk about some internal EVM details and look at known limitations for smart contracts _(the latter will be a perfect segway to the next topic: oracles and layer 2-s)._&#x20;

## Agenda

* EVM introduction
  * Defining blockchain in terms of state transition
  * How decentralized state machine works
  * Transaction structure
  * Accounts
    * layout and fields
    * types of account
      * Externally owned account (EOA)
      * Contract Account (CA)
  * Messages and message calls
    * types of message calls
* Contract code execution
  * Execution Model
    * storage types
      * stack
      * memory
      * Account storage
    * message calls and return values
    * input and output of messages
    * Exceptions
    * Gas supply and refund
  * EVM instruction set
    * looking at some important instructions (CREATE, SHA3, MUL, DIV, SDIV...)
  * How bytecode is compiled
    * Different types of compilers
      * [Solidity](https://docs.soliditylang.org/en/v0.8.20/)&#x20;
      * [Viper](https://docs.vyperlang.org/en/stable/)&#x20;
      * [LLL](https://lll-docs.readthedocs.io/en/latest/lll\_introduction.html)&#x20;
* Structure of the smart contract code (Developer perspective)
  * Storage
  * Memory
  * Functions
    * internal, external, payable functions
    * View Functions
    * Constructor functions
    * build-in functions
  * Events and logs
  * _Hello world example (code)_
  * _Simple Number storage example (code)_
* Overview of the next topic: Solidity and advanced smart contract functionality

## Overview Of Sources

Slides for this section will be adapted from [Ethereum EVM Illustrated](https://takenobu-hs.github.io/downloads/ethereum\_evm\_illustrated.pdf) (a bit old but still relevant).\
Introduction to smart contracts: [Ethereum docs](https://ethereum.org/en/developers/docs/smart-contracts/).

[Anatomy of smart contracts](https://ethereum.org/en/developers/docs/smart-contracts/anatomy/) - from Ethereum docs as well, covers a lot of parts in detail.

[youtube video](https://www.youtube.com/watch?v=2nEPWmaYBfs) about EVM message calls. seemed interesting.\
