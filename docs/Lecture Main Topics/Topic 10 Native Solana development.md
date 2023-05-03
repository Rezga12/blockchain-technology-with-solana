# Topic 10: Native Solana development

In this section we will be discussing writing native programs on solana, without using anchor framework. The main goal of the section is to get the audience acquainted with the approach solana took in designing its programs (aka smart contracts). At this points student should already be familiar with basic rust functionality as it's already covered in Workshops and assignments, and how programs are developed with anchor.

## Agenda

* Revision of what we already know about programs
* Building an escrow Program
  * Intro and motivation
  * What is an escrow
  * Project Structure
  * Entrypoints
  * Implementing instructions

This Section will mainly be covering paulx's article abount an introduction to the programming on solna: [Programming on Solana - An Introduction | paulx](https://paulx.dev/blog/2021/01/14/programming-on-solana-an-introduction/). The article is quite in depth and intensive for begginners, but it gives really essential information.

here are some additional resources on writting solana programs:

[Overview of Writing Programs | Solana Docs](https://docs.solana.com/developing/on-chain-programs/overview)

[Building and Deploying solana smart contracts | Chainlink blog](https://blog.chain.link/how-to-build-and-deploy-a-solana-smart-contract/)

A deep dive on how program deployment works under the hood: [Program deploys | Solana dev blog](https://jstarry.notion.site/Program-deploys-29780c48794c47308d5f138074dd9838)
