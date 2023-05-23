# Assignment 01: Simple Rust Programs
### 6-8 hours

This assignment is fairly simple and doesn't contain a lot of theory about blockchain technologies. The main goal for the exercises is to get students acquainted to rust.

**Exercise 1: String Guessing Game**\
In This exercise students will have to implement a guessing game between a program and a user. The program contains a hash that users have to guess. Program can only answer one question thorough: Did the input string matched the target. the type of the function output is `Result`, so it may be `OK` or `Err`, if string didn't match entirely, the result is `Err` and it contains the number of characters that actually matched from the beginning of the string. students will have to use `match` statement to complete this exercise.

**Exercise 2: Converting from/to base58**\
In blockchain almost every type of binary data is represented as base58 sequence. see more info the format here: [Why Base58](https://learnmeabitcoin.com/technical/base58).\
students goal in this exercise is to write two functions, _(which are self explanatory)_:

* `to_base58(data: u8[]) -> &str`,
* `from_base58(input: &str) - u8[]`

The exercise is intended for students to get more familiar with working with strings in rust.

**Exercise 3: Linked List Stack**\
In this exercise students will have to implement a singly linked list (LIFO stack; Last In, First Out).\
The list should have the following methods:

* `new()` - creates a new list
* `is_empty(&self) -> bool`
* `len(&self) -> usize` - returns the length of the list
* `push(&mut self, element: T)` - adds a new element to the front of the list
* `pop(&mut self) -> Option<T>` - removes the last element from the list and returns it
* `peek(&self) -> Option<&T>` - returns a reference to the last element of the list
* `rev(self) -> SimpleLinkedList<T>` - returns a reversed list

Also, Stack should implement `From` trait for Vec, So SimpleLinkedList can be collected into a vector:

```rust
let vec: Vec<_> = simple_linked_list.into_iter().collect();
```

FromIterator trait, so it can be created from an iterator.

```rust
let stack0: SimpleLinkedList<_> = (0..5).collect();
let stack1: SimpleLinkedList<_> = vec![1, 2, 3].into_iter().collect();
```

Objective of this exercise is to get students familiar with generics, traits and heap usage in rust.

**Exercise 4: Circular Buffer**\
In this exercise students will have to implement a circular buffer, storing elements of type \&T\
The buffer should have the following methods:

* `new(size: usize) -> Self` - creates a new buffer with the given size (throws an error size is not valid)
* `read(&mut self) -> Result<&T, Error>` - reads the oldest element from the buffer (throws an error if buffer is empty)
* `write(&mut self, element: &T) -> Result<(), Error>` - writes a new element to the buffer (throws an error if buffer is full)
* `clear(&mut self)` - clears the buffer
* `overwrite(&mut self, element: &T)` - writes a new element to the buffer, overwriting the oldest element

Objective of this exercise is to get students familiar with references, lifetimes, enums & custom errors.

**Exercise 5: XOR streaming adapter**\
In this exercise students will have to implement a streaming adapter, that will XOR the input stream with a given key.\
The adapter should have the following methods:

* `new<Key>(key: &Key) -> Self<'a>` - creates a new adapter with the given key
* `munge_in_place(&mut self, data: &mut [u8])` - XORs the given data with the key
* `munge<Data>(&mut self, data: Data) -> impl Iterator<Item = u8>` - XORs the given data with the key and returns the result (Shouldn't matter whether the byte iterator's values are owned or borrowed)
* `reader(self, impl Read) -> impl Read` - returns a reader that will XOR the input stream with the key
* `writer(self, impl Write) -> impl Write` - returns a writer that will XOR the input stream with the key

These traits will be useful: `AsRef`, `Borrow`, `IntoIterator`, `Sized`, `Read`, `Write`. Objective of this exercise is to get students familiar with lifetimes, generics & traits.
