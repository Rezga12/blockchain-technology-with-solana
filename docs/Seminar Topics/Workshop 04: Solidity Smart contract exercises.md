### Workshop 04: Solidity Smart contract exercises
In this Workshop we will pick up some practice by developing several smart contract using different functionalities provided
by ethereum environment. Students will be writing these exercises in REMIX.

**Exercise 1: Go Fund Me With Ethereum**\
The most trivial from all smart contracts. initializer user will create a new contract, where other users can deposit ETH 
to fund his project. after deposited funds reach certain amount, funders will no longer be able to withdraw their deposits back, nor add more funds. 
and initializer user will be able to withdraw the collected amount.\
functions to be implemented:\
* initialize state - only initializer should be able to call this function
* fund - everyone should be able to call this function
* withdraw your fundings partially or completely
* view funders and their deposited amount
* view funding threshold
* Gather Fundings - only initializer can call this function and only after the funding threshold is reached

**Exercise 2: Go Fund Me extension: thresholds should be in `USD` value**\
How we will be achieving this when smart contracts only know about ETH and understand very few about real world currencies
and even fewer about their current price. Of course, we will be using `Chainlink` Price feeds discussed in **TOPIC 08**.
well it will be an easy extension really. we just need to enable price conversion function in our contract code. To achieve this
several steps will be taken:
* There are a lot of price feed contracts in different networks, so we have to find correct address for ETH/USD feed on 
sepolia network.
* then we have to call `latestRoundData` method of the price feed in our contract code
* after we receive the answer we have to do some calculations to convert provided `ETH` value to `USD`


**Exercise 3: Writing new contract to aggregate different fundMe campaigns:**\
Currently our contract only serves as a fund collector for one user - initializer. out goal is to make a generic contract
so that any user can create hiw own campaign after the contract is deployed. of course we could modify existing contract
and update the mapping object so that it also stores campaign address, but in this exercise we will use ethereum
[Composability architecture](https://www.moonpay.com/learn/defi/what-is-composability).\
We will be building new smart contract which will have the reference to the existing smart contract code, and deploys new instance
of it every time new user initializes the campaign pool. more details on how to do it technically will be added later.




#### References:
For using price feeds: https://docs.chain.link/data-feeds/using-data-feeds - pay attention to `AggregatorV3Interface` interface