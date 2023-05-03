# Topic 04: Keys, Addresses and Wallet Technologies

This topic will cover everything regarding cryptography behind digital signatures, overview keypair generation algorithms. How do crypto wallets manage multiple addresses and see some details about wallet technologies.

## Agenda

* Introduction
  * Public Key Cryptography
  * Private and Public Keys
  * Elliptic Curve Cryptography Explained
  * Types of curves on different blockchains
  * Digital Signatures
  * Base58 format
* Wallets
  * Wallet Technology Overview
  * Nondeterministic Wallets
  * Seeded Wallets
  * HD Wallets (BIP-32)
  * Mnemonic Codes and Seed phrases (BIP-39)
  * Examples of Modern Decentralized Wallets

## Overview Of The Sources

[How Ethereum and Solana generate public and private keys](https://chainstack.com/how-do-ethereum-and-solana-generate-public-and-private-keys/) - This article covers a lot of ground regarding keypair generations. If more in depth explanation is needed we will provide some research papers aswell.

key points:

* Can Ethereum private keys be imported on Solana?
* Can hackers brute force crack a private key base on public information?
* How likely are two users are assigned to the same public address?
* Are different blockchains using the same cryptography system?
* What is a seed phrase and how does it work?

Also Chapters 4 and 5 from [this book](https://github.com/bitcoinbook/bitcoinbook) will cover the most topics discussed in this section.

* [Chapter 4](https://github.com/bitcoinbook/bitcoinbook/blob/develop/ch04.asciidoc): Key-pairs and addresses
* [Chapter 5](https://github.com/bitcoinbook/bitcoinbook/blob/develop/ch05.asciidoc): Wallets technologies
