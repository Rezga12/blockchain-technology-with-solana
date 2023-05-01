### Workshop 21: Nft Escrow Program
This workshop will not be long, here we will be rewriting our previously implemented
escrow program to support NFTs. The students will be using `Anchor` again.

**References:**\
[Example of escrow with anchor](https://github.com/coral-xyz/anchor/tree/master/tests/escrow)

**Exercise Description:**
Supposedly Two users want to exchange NFTs of the same collection, First, the user creates an escrow account to store his nft
then another user sends the nft to escrow initializer and unlocks the stored nft on the account. In out program isntruction
we will have to check that verified creator and collection address match for both NFTs, also the collection is verified for
both nfts

**instructions:**\
* `initialize_escrow(nftMintAddress)`
* `cance_escrow(escrowAddress, nftMintAddress)` - user can cancel his escrow account any time
* `swap_nft(lockedAccountAddress, lockedNftAddress)` - user to exchange his nft for a locked one

**client functionality:**\
In addition with instruction wrappers, client libraries will have to implement fetching of the all existing locked nfts, for the 
DApp users to choose which nft they wish to swap.
