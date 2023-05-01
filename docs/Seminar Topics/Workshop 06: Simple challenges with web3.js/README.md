### Workshop 06: simple challenges with webs.js

this section will contain some problems and excercises with web3.js. the amount will
depend on how many I can come up with. so the list is incomplete.

#### 1) Simple System Transfer
    
* this is the simplest challenge for solana development, using `SystemProgram`-s
   transfer instruction to transfer some between accounts.
* during this challenge we also can talk a bit about system program instructions
   and see the transaction results in preffered explorer.

#### 2) Fetching Transactions: Identifying System transfer in a bunch of transactions
   * this challenge will require for student to fetch all transactions for a specified\
   wallet address and determine how many system transfers have happened on this account
   * The second part of the challenge will require for student to determine the net change 
   (SOL deposits - withdrawals) for this account, for the past month for example.

   

#### 4) Splitting instructions into different transactions

* first task will be to transfer sol from specified wallet to a bunch of different wallets
The list of required wallets and lamport amounts will be provided as a json file: 
```json
{
   "D7guPJgn2oy8wafU15gjgeEZh2C1Fqvaqzd2vV8M7YYD": 1000,
   "29zMU3FKQt7cSgfUK1rneDUc82R1hVPHoYfkhWa9L1uc": 500,
   ...
}
```
we wouldn't wanted to use one transaction per transfer as keeping track of 200 transactions would be
much harder than one. so you will have to fit all the instructions in one transaction.
##### second part:
* as you might know solana transaction data limit is 1232 bytes. from solana cookbook
```
The Solana network uses a maximum transactional unit (MTU) size of 1280 bytes, 
adherent to the IPv6 MTU open in new window size constraints to ensure speed and 
reliability. 
This leaves 1232 bytes for packet data like serialised transactions.
```
supposedly you have to transfer different amounts of SOL to 200 or 300 different wallets,
**SystemTransfer** instruction takes about 40 bytes, so you can fit about 30 system transfers in
a transaction. you have to figure out the way to split the instructions in several transactions
as efficiently as possible, also keep track of succeeded, failed and skipped transactions and 
retry them if necessary.

5) 