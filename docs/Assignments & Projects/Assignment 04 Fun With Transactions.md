# Assignment 05: Fun With Transactions
### 5-6 hours

In this assignment, through several real world use cases students will learn how to fetch, filter, parse and generate transactions for `solana blockchain`.\
Starter files will be provided in the `./src` folder. Through There will not be much of them for this assignment.\\

**References:**

* [Transactions | Solana Docs](https://docs.solana.com/developing/programming-model/transactions)
* [Facts about Transactions | Solana Cookbook](https://solanacookbook.com/core-concepts/transactions.html#facts)

**Surface Level Description:**\
Web3 projects often encourage users to do actions benefiting to them by offering some kinds of rewards in `SPL tokens` or `SOL`. Usually users have a period of time to do specific actions, whether it will be interacting with some DeFi platforms, stake SOL, tokens or NFTs, buy or hold an X amount of Assets. As you might know all the data is public on blockchain, so after the specified period of time is over projects can scan through all the confirmed transactions in this period of time, (for a past month for example), see who completed specified tasks (by who we mean `wallet addresses`) and distribute promised rewards. This assignment will contain a few tasks similar to the flow described above:

* Find out who is eligible for rewards by going through transactions for specific period of time
* Determine what kind of rewards and what amount each wallet is eligible for.
* Distribute Solana to the specified addresses
* Distribute SPL tokens for the specified addresses
* Distribute NFTs for the specified addresses
* making sure that all sent transactions have been confirmed and retry failed or skipped ones

Students can airdrop some solana on `devnet` for testing purposes, although the querying part of the assignment will most likely take part on `mainnet-beta` due to the fact that there's more diverce data and we can come up with more interesting use cases.

## Exercise 1:

This exercise will be fairly simple, Eligible wallets will be provided in advance and payouts will be in `SOL`. The main reason for this exercise will be to make student acquainted with the flow of sending multiple transactions and querying for their statuses. the next excersises will be somewhat more challenging.

## Exercise 2:

Here users will have to find out which wallets are eligible for the payouts, also payouts will be in SPL tokens so instructions will take some extra steps, if the users doesn't have an associated accounts for the token we will also have to create it for them.\
Ideas for the rules:

* wallets with the most SOL circulation
* wallets who hold more than `X` amount of spl token `Y`, the amount to pay out will be proportional of the fraction the wallet holds
* wallets who hold more than `X` NFTs from the specified collection. The payout will also be proportional to the number of nfts they hold Or there will be some threshold values.

## Exercise 3:

In previous exercises the rules were dependent on current state of the blockchain, Here the rules will include what user did in the past `X` period of time or from specified date to specified date.\
Possible Ideas:

* Wallets which held more than X amount of specified token or nft for the past month
* Wallets which minted an NFT of specified collection
* Wallets which staked more than x tokens for more than x amount of time
* wallets which interacted with specified Decentralized applications more than x amount of times

The main point of this Exercise is for students to learn querying and parsing transactions. the payouts in this exercise will be held in SOL, SPL token transfers and account creations are covered in previous exercise.
