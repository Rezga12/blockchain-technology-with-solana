## Topic 8: Solana Transactions

This Section goes through solana transaction overview, as we know every operation on a blockchain
needs transaction submitted to the cluster. We explain how is transaction received, processed and commited
by the cluster. We will also look at transaction anatomy and what disect it's data model

### Agenda

* Overview Of A transaction
* Anatomy of a Transaction
  * Transaction Format
  * Instructions format
  * Signatures
  * Account addresses format
  * Compact array 
* Instructions
  * Instruction data
  * program Id
  * Accounts data
* Finality and Confirmation (Confirmed vs Finalized vs Skipped)
* What is a Blockchash and how it's used in transaction
* Signers
* Fees and fee payers
* Communicating with RPC nodes
* How are transaction ids generated
* Using Solscan To analyze Basic Transactions
* Getting comfortable with analyzers like solscan or solana.fm
* show transactions of our pseudocode programs and demystifing them

### Overview Of The Sources

* [Transactions | Solana Docs](https://docs.solana.com/developing/programming-model/transactions)
* [Transactions | Solana Cookbook](https://solanacookbook.com/core-concepts/transactions.html#facts)

Mapping solana transaction field to ethereum ones & underlining differences and similarities:
[Transaction | Solana Wiki](https://solana.wiki/docs/solidity-guide/transactions/#solana-transaction-structure)

Introduction of Transaction fees and Account Rend:
[Transaction Fees | Solana Docs](https://docs.solana.com/developing/intro/transaction_fees)

A bit more of a deep dive on how are fees calculated: [Fee Determinism article](https://jstarry.notion.site/Transaction-Fees-f09387e6a8d84287aa16a34ecb58e239)

Medium article about what a serialized transaction model looks like:

[Solana Transactions in Depth](https://medium.com/@asmiller1989/solana-transactions-in-depth-1f7f7fe06ac2)

Articles about transaction Finality Statuses, general issues and why transactions get skipped:
* [Transaction Confirmation](https://jstarry.notion.site/jstarry/Solana-Dev-Blog-302b7e08652c4a2dbc0be4f6a3b0d317?p=d5b8f4e09b9c4a70a1f263f82307d7ce&pm=c)
* [Retrying Transactions | Solana Cookbook](https://solanacookbook.com/guides/retrying-transactions.html#facts)

Popular Explorers, differences and which one to use:

* https://solscan.io/
* https://explorer.solana.com/
* https://solana.fm/

Common terminologies:
* TPS
* Current Block
* Block Hash
* Transaction Id
* How to track network problems
