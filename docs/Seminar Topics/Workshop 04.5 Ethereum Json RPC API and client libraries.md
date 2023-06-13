### Workshop 04.5 Ethereum Json RPC API and client libraries
In this workshop we will go through all the available methods on how users can query and interact with the ethereum blockchain.
Also, we will look at some go to etherium javascript client libraries lik `Ethers.js` and `Web3.js`, will talk about them,
underline similarities and differences between them and why there are two of them when all the other blockchains have only one
main client library to work with. We will also review some examples and do exercises where students will have to utilize
these libraries.

**References:**
* [JSON-RPC API | Ethereum docs](https://ethereum.org/en/developers/docs/apis/json-rpc/)
* [Execution API specification | github](https://github.com/ethereum/execution-apis)
* [Etheres.js vs Web3.js comparison](https://dev.to/lparvinsmith/web3js-vs-ethersjs-a-comparison-of-web3-libraries-2ap5)
* [Etheres.js](https://docs.ethers.org/v5/)
* [Web3.js](https://web3js.readthedocs.io/en/v1.10.0/)

#### Table of contents

* RPC-API some methods worth noting
  * `eth_getBalance`
  * `eth_getCode`
  * `eth_getTransactionCount`
  * `eth_call`
  * `eth_sendTransaction`
  * `eth_getTransactionByHash`
* Practice small exercises

The main methods here are `sendTransaction` and `call`, it enables us to send transactions to the chain. 


**Exercise 1: fetch specified wallet balance:**\
very simple exercise, we will learn how to send some ETH from one wallet to another.

**Exercise 1: fetch and parse transactions by hash**\
We will learn how to fetch transaction data given the transaction hash. students will have to inspect fields of the 
returned output and see what fields they can inspect.

**Exercise 2: interact with our `Fund Me contract`**\
We will have to use web3.js to interact with previously written and deployed fund me contract, to create campaigns,
fetch all the existing campaigns and fund them, also withdraw collected funds and see the transaction outputs.

more exercises to be added...
