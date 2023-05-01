### Assignment 06: Simple decentralized Exchange
In this assignment students are required to build a decentralized exchange, using **_Constant function automated market maker 
method_** (CFAMM for short). The main challenge is to write a solana program to support all the functionality needed to 
make our DEX work.\
Students will be using `Anchor` framework for building the program as well as the frontend client.
starting files will be located in `./src` folder, but there will not be much of them.

**References:**
* [Constant Function Market Makers: DeFi’s “Zero to One” Innovation](https://medium.com/bollinger-investment-group/constant-function-market-makers-defis-zero-to-one-innovation-968f77022159)
* [Overview Of Uniswap markets | Stanford](https://arxiv.org/pdf/1911.03380.pdf)

**Surface Level Introduction**\
Although we won't go into much detail to optimize our solution, we will have to understand how constant product AMMs work,
what is slippage, how is liquidity generated and etc. Theese topics will be covered in lectures and seminars, so students will
have all theoretical knowledge they need to implement this task.

**The Program:**\
Implementing a smart contract will be the main part in this assignment, the basic functionality our program should have are:
* a way of creating liquidity pools, for different tokens, there are several ways of doing this:
  * An authorized wallet address or a list of authorized wallet addresses should be able to create pools without needing to provide liquidity
  * Everyoune can Create pools, but they should provide a decent amount of starting liuiquidity
  * An assignment may contain both ways combined or separately.
* a way for users to provide liquidity, meaning putting two tokens of the same value. the user chooses amount for one token,
and the amount of another is determined by our program.
* A way for traders to swap tokens at active pools, maintaining constant function and balancing prices. also Distributing
fees to the liquidity providers and the platform
* The minor detail but, will add if assignment doesn't come out too complex: Wrapping and unwrapping `SOL`, to make it easier 
to implement logic for pools with solana and doesn't make it different from other SPL tokens.
* will add if I left some core details...

**The Client:**\
the client library will be wrapper for program instructions as well as querier for current state of the AMM. the UI is not
required from students, there might be a basic UI provided for them in form of single page application and students will have to
implement UI component handlers to interact with program.



