# Workshop 19: Nft Marketplace Program

In This Workshop we will implement the program and the client side of a simple NFT marketplace. Payments will be held in Solana as well as specific SPL tokens. Probably the implementation of each instruction will be the separate exercise for students.

**References:**\
you can view [Magic eden](https://magiceden.io/) to get a grasp of how nfts work on solana generally

## Instructions:

**List Nft In Solana:**\
The core instruction for marketplace program, aside from account addresses instruction should take listingPrice as an argument: `list_nft(price)`.\
Checks that user should take into a consideration:

* is user the owner of the NFT
* The nft is the part of the collection allowed on our marketplace
  * for check to be possible we should also keep the list of allowed collections somewhere
* the nft is correct metaplex asset class (it might be the fungible asset that we don't want to support)
* check that pda account designated to store an NFT is correctly passed.
* check that specified price is not too low (0 for example)

**Cancel Listing:**\
If the nft is listed an nft owner should have a possibility to delist it, in order to get his NFT back.\
instruction signature: `cancel_listing()` Checks for validity of the arguments:

* Validate that listing initializer is the signer of the instruction
* Validate that other accounts (nftMint, tokenAccount, etc) are also correctly passed\
  Other than that it's pretty strait forward implementing this instruction.

**Buy NFT:**\
Instruction should subtract the nft price amount of SOL to the (signer) and send him an NFT.\
**Royalties:** each nft has list of creators in its metadata, our instruction should respect the creators of the colleciton and distribute royalties according to it. the creator fee should be subtracted to the price so seller might not receive the exact price of the nft. we can also have the marketplace fee as well for ourselves. Checks that students should take into consideration:

* validity of passed accounts (metadata, associatedAccounts, etc.)

**Update Price:**\
This instruction is usually also implemented in marketplace contracts, it lets user update price without listing the account. The only logical check you need to make is to match the signer with the account initializer and check if the price is not too low.
