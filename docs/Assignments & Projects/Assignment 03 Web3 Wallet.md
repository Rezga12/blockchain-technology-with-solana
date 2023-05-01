### Assignment 03: Web3 Wallet

In this assignment students will be required to implement Web3 wallet functionality for solana using **Typescript** and
`@solana/web3` library\
Starter files will be provided in the `./src` folder.\

**References**:
* [What is a Wallet | Solana Docs](https://docs.solana.com/wallet-guide)
* [Command Line Wallets | Solana Docs](https://docs.solana.com/wallet-guide/cli)
* [Web3 JavaScript API | Solana Docs](https://docs.solana.com/developing/clients/javascript-api)

**Surface Level Description:**

Modern DeFi wallets have few core functionalities:
* Create Wallet with the new seed phrase
* Create Wallet With already existing seed phrase
* Securely Save Private keys and seed phrases
* Manage Multiple `keypairs`
* Display Solana Balance
* Display Other SPL Token Balances
* Display Net Worth of all Tokens
* Send SOL or any other SPL token to specified address
* View the Latest Transactions of a wallet
* Sign Transaction on other dapps
* (Extension) Display and Send NFTS

There's quite a lot of functionality, the assignment will not necessarily
contain all of those. Some functionalities will be already implemented in starting project
in order to help students understand how the library works.\
In ideal case the project will have a form of the `google chrome` extension. Students will
not have to learn how extensions work, that part will already taken care of.\
UI will also be implemented in advance, students will have to work with the methods invoked
after some UI actions. For example when user logs in to the wallet, Net worth of the user, that
is the dollar value of all tokens is displayed in the biggest font:
![](https://pbs.twimg.com/media/E9AW7zeUYAEcOMA.jpg)
Students Will just have to implement `getNetWorth()` method in typescript, which will
return a number equal to the dollar value of all the tokens user has on an account.\
Other functionalities will be implemented in similar way. Of course the most part of technical 
details, will be covered in assignment document, but not all the parts. For some functionalities students
will be required to search the web on their own. 

If we find out that building starting files as a chrome extension is too complicated
to test and work with, the project will be a single page web app with a simple ui, like
[Solflare](https://solflare.com/) web wallet.

