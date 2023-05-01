## Topic 6: Solana Accounts and Programs

This Section starts with an introduction to solana account model, types of accounts and 
their characteristics. Underlining that Accounts are something like first class citizens on solana and
they take place in almost every process on solana.
Programs are also discusses on this Section, but only partially. developing custom programs
are looked at in later sections.
from this section lectures will take more developer sided approach rather than eductaional one.

### Agenda

* Solana Accounts
  * Types of accounts:
    * Data accounts
      * System owned accounts
      * PDA accounts
    * executable(program) accounts
    * native accounts
  * Rent and Rent Exemption
  * Account layout and data model
  * Read Only and Writeable Accounts
  * Creation of accounts
  * Account ownership and assignment to programs
  * Sealevel Runtime Account Rules
  * Discussing Examples of simple accounts
* Solana Programs
  * Overview Of Solana Program ideology
  * How are programs and accounts related
  * Native Programs vs On Chain Programs
  * Program ownership and upgrade authority
  * Overview(not in depth) of Program deployment process 
  * Solana Program Library (SPL)
  * Important SPL programs:
    * Example: Token program
  * What is Composability and parallels with solana programming model
* Example of a solana program (With Pseudo code)
  * Showing the execution of the program conceptually
  * [example programs to show pseudocode of](https://github.com/coral-xyz/anchor/tree/master/examples/tutorial)


### Overview and Sources

#### Accounts:

* [Accounts | Solana Docs](https://docs.solana.com/developing/programming-model/accounts)
* [Accounts | Solana Cookbook](https://solanacookbook.com/core-concepts/accounts.html#facts)

Types of Accounts:
* Data accounts store data
* Program accounts store executable programs
* Native accounts that indicate native programs on Solana such as System, Stake, and Vote

* System owned accounts
* PDA (Program Derived Address) accounts

Here we also can explain what are PDA addresses, How to generate and interact with them:
[Deep Dive on PDAs | Solana Cookbook](https://solanacookbook.com/core-concepts/pdas.html#facts)


[A Deep Dive into Solana Account Model (1) — Introduction](https://medium.com/@lianxiongdi/a-deep-dive-into-solana-account-model-1-introduction-7b0408656593)

This article doesn't align with The section topic exactly, but might still be interesting to mention:
[Solana Composability vs Ethereum Composability](https://blog.strataprotocol.com/solana-composability-vs-eth-composability)


#### Programs:

* [Programs | Solana Cookbook](https://solanacookbook.com/core-concepts/pdas.html#facts)
* [Programs | Solana Docs](https://docs.solana.com/developing/programming-model/accounts)

[Technical overview of program deployments](https://jstarry.notion.site/Program-deploys-29780c48794c47308d5f138074dd9838)

Solana Program Library docs: https://spl.solana.com/


A high-level overview of the account model in Solana’s runtime called Sealevel:

[Solana Wiki | Accounts](https://solana.wiki/zh-cn/docs/account-model/#account-storage)


