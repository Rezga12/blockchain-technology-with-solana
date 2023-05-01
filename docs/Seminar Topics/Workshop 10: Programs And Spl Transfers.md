### Workshop 10: Programs And Spl Transfers
In This workshop we will dive a bit deeper with solana programs, by introducing operations
on SPL tokens and accounts.

**Excersise 1: creating wrapped Solana**\
As you might already due to the fact that solana is native token, transfers
operations on it happens differently than on SPL tokens. Because of this programs need a lot 
of branching in their code to handle `SOL` and `SPL tokens` separately. A good workaround for this
is a notion of wrapped SOL. It's really popular for decentralized exchanges like [Raydium](https://raydium.io/):
It's when you receive an amount of specific Token in exchange for the same amount of `SOL`. for this
exercise we will write a simple program to help users exchange their solana for some SPL token
that will be stored on PDA associated token account. program will have four instructions:
* `wrap_sol`
* `unwrap_sol`
* `deposit_sol` - this instruction will be to replenish solana balance on program account
* `deposit_w_sol`- same one as above but for SPL token
Only the specific whitelisted wallets should have an ability to replenish the balance,
but everyone can wrap or unwrap their solana.

**Exercise 2: An Escrow Program**\
definition of escrow: `a bond, deed, or other document kept in the custody of a third party and taking effect only when a specified condition has been fulfilled.`
This is a common use case for blockchain applications:\
Supposedly Alice has an X amount of USDC and Bob has Y amount of BONK, they want to
exchange their tokens without trusting each other, and also without relying on the third party authority.\
We should write a program to accommodate the exchange.

There should be several simple instructions:
* `initialize_escrow(offered_amount, requested_ammount)` - initializer has to create a program account which will store metadata about the transfer.
and of course lock the amount of tokens he wishes to offer to the second party.
* `cancel_escrow(escrow_address)` - escrow initializer should be able to cancel the offer and close the
account any time.
* `accept_offer()` - This instruction will be called by second party to accept the offer and trade tokens.




