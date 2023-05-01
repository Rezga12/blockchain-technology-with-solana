### Workshop 10: Building Solana Programs
This workshop will be somewhat an introductory part about programs and will contain 
technical details about developing and building programs(as the subject is covered theoretically on the lecture).
Also, a pseudocode will be displayed on the first lecture, while only real anchor programs will
be deployed and tested on workshops.

**The Topics covered on the workshop:**
* setting up `anchor cli tools` (students already should have rust toolchain set up as earlier excersises were on rust)
* Going through anchor project structure:
  * `src` directory
  * tests directory
  * target directory
  * explaining `Anchor.toml` file
* Write the simplest solana program with anchor, explaing what's going on
* Test that what we wrote is working by deployinh and testing the program

**Exercise 1: Ensure that anchor is set up and programs can be developed and deployed**\
first exercise will be somewhat default one: to set up the anchor environment and deploy
first program on `devnet`.

**Exercise 2: Simple Logger Program**\
This is the simplest solana program possible. it only has one instruction:
* `log_input(string)`\
it logs the text sequence specified as a parameter. also the instruction should fail
when the string length is greater than some arbitrary number

The above instruction will be implemented by the lecturer, students will have to implement the next two
instruction:
* `set_max_length(newMaxLength)` - set the max allowed length of the log string
* `set_log_prefix(setLogPrefix)` - set the static string prefix that should be logged with the specified string
This will be the first time students will be implementing instructions, so they are fairly simple.
* 

**Exercise 3: Solana Number Incrementor**\
Unlike the previous one, this program will not be stateless and will have one account to store a single number.
the program will have the following instructions:
* `create_number_store_account()` - creates the program PDA account
* `increment_number()` - increments the stored number

This two parts will be implemented by the lecturer, Stuents will have to change the program to 
comply with specified needs:
* The number for different users should also be different _(working with PDAs)_
* add some more operations like subtraction, addition of an arbitrary number, multiplication etc.
* implementing `close_account` instruction.


**Exerciese 4: Solana Locker Program**\
The program only contains two instructions:
* `lock_sol` (The instruction will be implemented by lecturer)
* `unlock_sol` (The instruction will be required to be implemented by students)

only user who locked their funds will be able to unlock them.
This program is a bit far from real world use case but it will be good for education purposes.

This programs will be enough for students to get a grasp of it. The workshop may span 2-3 seminars
if the explanation comes out too long.
