# Assignment 03: Merkle Distributor for Airdrop

In this Assignment students will be implementing a small airdrop program, first with linear wallet storage and then with **merkle tree distributor** for validating eligible wallets for airdrop.\
Starting Files Will be located in `./src`

**References**:

* [A Cumulatibe Merkle Distributor for Airdrop | Medium Article](https://pngfi.medium.com/a-cumulative-merkle-distributor-for-airdrop-51f0a5b49d2c)
* [Merkle Distributor | Github Repo](https://github.com/pngfi/merkle-distributor)
* [What is Rent | Solana Docs](https://docs.solana.com/developing/intro/rent)

**Surface Level Description:**

## Part 1

When conducting an airdrop tp a large number of users, the typical approach is to store user's wallet addresses in a program, and claims are initiated by the users. The first part of the assignment will be constitying of just that part. Students Will Have to build a program that can store wallet addresses, and amount of `SOL` the wallet address is eligible to receive. Users than will initiate the `receive_airdrop` instruction, where program will check if the user is qualified for airdrop and if all checks are passed, send him the sufficient `SOL` from its Treasury account.

## Part 2

The Second Part Of the assignment will be consisting of putting the use to the merkle tree functions students wrote in the previous Assignment. Here we should write new Program, which stores Merkle root for all the wallet addresses, and then require a `Merkle proof` when users try to initiate `receive_airdrop` instruction. This approach better in terms of storage and `Rent` costs. Additional details for constructing this assignment is in medium article linked above.

## Part 3

It's also a good idea to have students calculate how much rent they saved by going with approach number two, given the static list of wallet addresses.
