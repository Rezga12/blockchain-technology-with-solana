### Workshop 03: Smart contract Development with Remix IDE

in this workshop we will cover technologies around smart contract development on **Ethereum**. First we will look at
[REMIX](https://remix.ethereum.org/#lang=en&optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.18+commit.87f61d96.js) -
_a powerful toolset for developing, deploying, debugging, and testing Ethereum and EVM-compatible smart contracts_. We will also
learn how to use https://etherscan.io/ - to track our created contract transactions.

**Table of Contents**\
* Remix IDE overview
  * File Explorer
    * discussing project structure
    * creating new file for our contract
  * Solidity Compiler
    * choosing different compiler version
    * how to compile written contract code
    * view the generated files after compilation
  * Deploying smart Contract
    * Choosing between different environments
    * What is Remix Javascript VM
    * How to connect to the real testnet network
    * deploying contract to VM
    * deploying contract to Sepolia network
  * Building and explaining simple Storage smart contract

Exercise 1:\
Hello world program. it only has one instruction: `getHelloWorldText` - which returns one string:
hello world text.

Exercise 2:\
Build simple smart contract using solidity with really basic functions:
* ability to store array and mapping of integers
* ability to update mappings with transaction
* ability to retrieve value from mapping by specified key

View deployed contract on Etherscan and view it's transactions.

#### References:
* [REMIX Documentation](https://remix-ide.readthedocs.io/en/latest/)
* [Ethereum different networks](https://ethereum.org/en/developers/docs/networks/)
* [Etherscan | Sepolia](https://sepolia.etherscan.io/)