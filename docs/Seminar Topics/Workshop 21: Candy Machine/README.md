### Workshop 21: Candy Machine
The Metaplex Protocol **Candy Machine** is program that has functionality which helps to distribute NFTs fairly during the
new collection launches. Metaplex Docs includes all the information about candy machines including theory as well as practical
examples. On Seminars, we will talk about the architecture of a candy machines and then complete some exercises
together with students.

**Workshop Agenda:**\
* Candy Machine Overview
  * Why candy machine
  * The lifecycle of candy machine
  * Candy Guards
    * How candy guards work
    * Overviewing most popular candy guards
    * Guard Groups and different minting buckets
* Setting up candy machine
  * Candy Machine Settings
    * config line settings vs hidden settings
    * why they use hidden settings
  * How to upload items
  * How to start minting process publicly
  * How to manage whitelists
  * Did anything change with the introduction of Programmable Nfts

After theoretical part students will be given exercises to get acquinted with candy machines. This workshop will also span
more than one seminar.

**Exercise 1:**\
Publishing a candy machine with [Candy Machine CLI: Sugar](https://docs.metaplex.com/developer-tools/sugar/overview/introduction).
There is a corresponding [tutorial](https://docs.metaplex.com/programs/candy-machine/how-to-guides/my-first-candy-machine-part1) 
on Metaplex website, that follows the same steps students will be following on their workshop:
* Install Sugar
* Set Up Your Project directory structure
* Create a Config File
* Uploading Images and Metadata to External Storage
* Deploy a Candy Machine
* Verify Successful Deployment
* Mint an NFT

But that's not enough, we also should write a bit of client code to make it easyer for
users to mint NFTs. Here we will be using Candy Machine js library to provide the needed functionality.
The client will propbably contain only one method for the starters:
`mint_nft`

**Exercise 2:**\
In this exercise students will have to do the same but this time instead of `Sugar` they will be
using [Metaplex JS SDK](https://github.com/metaplex-foundation/js).
Here's [corresponding tutorial](https://docs.metaplex.com/programs/candy-machine/how-to-guides/my-first-candy-machine-part2) just with the exercise 1.
Right now JS is the way to go when creating candy machine instances, due to the fact that it provides
complete functionality, for example, with sugar you can't upload just urls of the metadata accounts.
May be sugar will be enhanced in the future but right now JS SDK is much more mature for candy machines.

The additional part with difference of first exercise will be adding guards to the created candy machine.
we will add [Bot Tax](https://docs.metaplex.com/programs/candy-machine/available-guards/bot-tax) 
and maybe [Token Payment](https://docs.metaplex.com/programs/candy-machine/available-guards/token-payment) 
or [Nft Burn](https://docs.metaplex.com/programs/candy-machine/available-guards/nft-burn) guards.
more info about guards: https://docs.metaplex.com/programs/candy-machine/candy-guards


