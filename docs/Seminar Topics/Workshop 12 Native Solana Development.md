# Workshop 13: Native Solana Development

In previous workshops we covered building and deploying programs with anchor framework. usually learning path goes other way around: student first learns the specific technology, and after he has some understanding of that technology he starts learning the framework built upon the technology. But we went the other way and chose to use top-down approach, in my opinion the basic concepts of program smart contract development is easier to learn with anchor, and after you have some grasp of what's happening you will be learning what is happening under the hood.

Well This workshop will not have much of the description. A lot of theory is covered in Topic 10. We will just implement some programs we have already written in previous seminars using `Anchor`. Students will have a chance to observe how different is the implementation of the same functionality with using only the native libraries.

**Exercise 1: Simple Logger Program**\
This is the simplest possible program that can exist on solana. and we have already written it using anchor. Now it's time to develop it using solana native libraries.

**Exercise 2: Solana Locker Program**\
Just as the last time this program just locks solana to the program account and user can release it any time. the important part is to track how much sol each user has locked in the program. Students will be learning account management using native solana libraries.

**Exercise 3: SPL token transfers**\
Creating Wrapped solana was fairly easy challenge with the help of the anchor framework. But when only option is the native libraries it might be a bit challenging.

There Is not a specific exercise involving cross program invocations, but I think Exercises 2 and 3 cover CPI contexts just as well.
