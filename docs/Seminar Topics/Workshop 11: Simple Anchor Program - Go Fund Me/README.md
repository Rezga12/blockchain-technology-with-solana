### Workshop 11: Simple Anchor Program - Go Fund Me
This program is a bit larger than the exercises in previous sections. it requires a lot more
PDA management. Implementing This program will span several seminars and some part will be implemented 
by students and some part will be implemented by lecturer, some will already be ready as 
starting files.

The main idea of the program is to collect funds from different wallet addresses,
when the specified threshold is met the funding will be closed and the initializer can
collect the funds.
so program will have different instruction of different participants of the process:
* `initialize_funding_account` - any user can initialize their account and request funding
* `cancel_funding_account` - user can cancel the funding and no more users will be able to deposit funds
  _(also an idea for interesting extension will be to close account and distribute the funds back to the
funder users)_
* `fund_campaing(campaingAddress, amount)` - user transfers his funds to the campaign account
* `revoke_funding(campaingAddress,)` - user can withdraw funds any time before the threshold is reached

**The Client Library**\
The client library will be implemented with `@coral-xyz/anchor` typescript package with of course
has a dependency on `@solana/webs.js` - the library we are already familiar with.\
The main functionalities of client library will be:
* fetch all campaigns
* fetch user created campaigns
* fetch user funded campaigns
* fetch active campaigns

This type of client functionality is quite common in blockchain applications working with smart contract state.