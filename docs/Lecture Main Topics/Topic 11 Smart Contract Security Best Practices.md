# Topic 11: Smart Contract Security Best Practices

This topic covers all common security risks developers need to take into consideration when writing smart contracts. We will also talk about best practices to avoid those security risks

## Agenda

* Known Vulnerabilities on ethereum
  * Reentrancy attacks
  * frontrunning
  * why these attacks are possible only on ethereum and not on solana
* Overview of known vulnerabilities on solana
  * Missing ownership check
  * Lack of signature validation
  * Integer overflows and underflows
  * failure to validate external programs
  * Loss of Precision
  * Program substirution
* Several Case analysis
* How anchor helps with security vulnerabilities
* Sealevel attacks on anchor

## Overview of the sources


#### front running:
* [Ethereum frontrunning transactions](https://consensys.github.io/smart-contract-best-practices/attacks/frontrunning/)
* [Front running | SOlidity by example](https://solidity-by-example.org/hacks/front-running/)
* [Analysis of ethereum front running sandwitch and it's known defence solutions](https://medium.com/degate/an-analysis-of-ethereum-front-running-and-its-defense-solutions-34ef81ba8456)


#### reentrancy attacks
[Hack Solidity: Reentrancy attack](https://hackernoon.com/hack-solidity-reentrancy-attack)

#### solana vulnerabilities
Repo dedicated to smart contract security best practices: https://github.com/slowmist/solana-smart-contract-security-best-practices

[Solana Smart Contracts: Common Pitfalls and How to Avoid Them](https://blog.neodyme.io/posts/solana\_common\_pitfalls/)

github repo: [coral-xyz/sealevel-attacks](https://github.com/coral-xyz/sealevel-attacks) where some possible exploits and their recommended safety checks are given.
