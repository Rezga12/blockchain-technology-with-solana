# Topic 09: Writing Programs with Anchor Framework

Program Development basics will start with introducing anchor framework. In my opinion it will be better for grasping core smart contract concepts. native solana development has stiffer learning curve, and it surely requires some deeper knowledge. we will learn native libraries after we will have some practice with anchor.

## Agenda

* Introduction
  * What is Anchor
  * High Level overview
* Core Concepts
  * The Accounts Struct
  * The Program Module
  * Custom Errors
  * Cross Program Invocations
  * PDAs
  * Interface Description Language (IDL)
    * How IDL is deployed
* Developing With Anchor
  * Anchor tools
    * anchor-cli
    * anchor version manager (avm)
  * Anchor Project Structure
  * Workspace walkthrough
  * building and deploying with anchor
  * Anchor client library
  * Writing unit tests with mocha
* Anchor client library
  * Typescript package on npm: `@coral-xyz/anchor`
  * writing client code for already existing program

## Overview of The Sources

Anchor github repo: https://github.com/coral-xyz/anchor Anchor website: https://www.anchor-lang.com/ Anchor book: https://book.anchor-lang.com/

additional tutorials:

* [Build a blog dApp using the Anchor framework](https://learn.figment.io/tutorials/build-a-blog-dapp-using-anchor)
* [Introduction to Anchor | SolMeet](https://book.solmeet.dev/notes/intro-to-anchor)
* [Deep Dive into Anchor by Implementing Token Management Program | SolMeet](https://book.solmeet.dev/notes/anchor-token-management)
