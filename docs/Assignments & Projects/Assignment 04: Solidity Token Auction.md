### Assignment 04: Solidity Token Raffle Auction.md

### 10-12 hours

this assignment requires for students to write ERC20/ERC721 token auction smart contract, where bidders pay ETH to compete in winning
auction. or it might be the other way around, they bid specific ERC20 token to win specified Nft.

**References:**\
[Chinese Auctions aka Raffles](https://www.onecause.com/blog/chinese-auction-definition/)


**Description:**\
The raffles are very common in DeFi projects, Contract owners often announce raffles, where users
are competing to win some NFT or an amount of tokens. The users have to buy tickets to participate in a raffle,
each ticket costs some amount of ETH or USDC, users can lock their tickets in a raffle, and when the deadline
comes one ticket will be picked randomly as a winner. It's something like a lottery.

**The Functionality:**\
there will be two parts in this assignment: Give dapp users ability to buy raffle tickets,
and Give users ability to lock those tickets in expectancy of rewards.\
First part will be implemented in distinct contract called `Ticket Manager` contract.
* create new `ERC-20` token, with decimal count of `0`, which will correspond to a raffle ticket,
this standard is called semi-fungible token, where tokens have metadata attached to it, but they are fungible.
* `buy_raffle_ticket` - this will be a payable function in our contract. it will receive `ETH` and 
send the buyer back our `$TICKET` token proportional to the `ETH` value they sent to a contract.
* `set_ticket_price` - ticket price should be configurable by the contract creator.

**Second part:**\
these functions will be the part of the distinct smart contract. We will call it `The Raffle` contract.
* `lock_tickets` - by calling this function signer will transfer the specified amount of raffle tickets
aka $TICK token to the contract.
* `initialize_raffle` - initializes information about raffle, like what is the reward, what is the start date and end date of the raffle
end etc.
* `start_raffle` - calling this function should start the raffle despite the configured start date.
* `set_raffle_end_date` - this function changes the configuration of the end date of the raffle

**Third Contract: Raffle aggregator**\
`The raffle` contract discussed in the second part will only contain the information about one specific raffle event, we need third contract which will
allow the DAPP owners to create new event whenever they want with the specific configurations. for this we will be needing the third contract which will have
the reference on all ongoing, finished and upcoming raffle events in terms of smart contracts.\
Functions:\

* `create_raffle_event` - this function call will create and deploy the instance of the new `Raffle` smart contract
* `initialize_raffle_event` - we need to pass the contract ID of the raffle we need to configure.
* Other methods will be wrappers for the previous contract, with one additional parameter: the contract ID.

All the contracts specified above should be developed and tested using remix IDE. There might be requirement for implementing 
client library with javascript, if we decide to increase difficulty of the assignment, or require students to use [Hardhat](https://hardhat.org/) 
environment.
