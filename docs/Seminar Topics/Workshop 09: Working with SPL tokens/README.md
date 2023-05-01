### Workshop 09: Working with SPL tokens
In this workshop students will get hands-on experience with working with SPL tokens, associated accounts and mints. generally
how solana account model manages SPL tokens.\
We will mainly be using `web3.js` library together with `@solana/spl-token` package to solve some excersises.

**References:**
* [Token Program | Solana Docs](https://spl.solana.com/token)
* [Associated Token Account Program | Solana Docs](https://spl.solana.com/associated-token-account)
* [A Deep Dive into Solana Account Model (2) — SPL Token](https://medium.com/@lianxiongdi/a-deep-dive-into-solana-account-model-2-spl-token-d029d97aa6e0)
* [Solana SPL token npm package](https://github.com/solana-labs/solana-program-library)

**Quick Workshop Summary:**\
At this point we already know how to create an SPL token using cli tools (from the previous workshop), as well as some basic stuff about SPL tokens.
So as the first exercise we can do everything we did before but using typescript.

**Exercise 1: Basic SPL token creation**\
Mint new SPL token using `@solna/spl-token` library. token should have next properties:
decimals: 9,
maxSupply: 100000
freeze authority: token creator wallet.
students also have to generate token transfer transactions to create accounts and transfer their tokens to other wallets.

**Exercise 2: Associated Token Accounts**\
First we will have a little introduction about associated accounts and why we need them. Look through the instructions
of `associated token account` on [github](https://github.com/solana-labs/solana-program-library/tree/master/associated-token-account/program/src)
Therese are only 3 of them, so we will explain why we need them and why we even need a program
to manage token accounts with specific seeds.

Students will have to write a query to fetch all the token balances for specified wallet address.
The querry should also display what are the specified tokens on the accounts, for example
is it `$USDC`, `$USDT`, `$wSOL`, `$BONK` or something else? We will also look at the ways of determining
that.

**Exercise 3: Creating SPL Token Metadata**\
In previous excersise we learnt how to determine if token metadata exists and fetch it. Now students will
learn how to set metadata for tokens created by them in the first exercise. THey will also learn how to upload
their token off-chain on a [Decentralized file storage - Arweave](https://www.arweave.org/), If the task is completed properly
students should be able to see their token image and name in any wallet which connects to Devnet.







