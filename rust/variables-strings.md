# String variables in Rust

A computer understands a string to be a set of bytes guaranteed (in Rust) to be valid UTF-8 (character encoding). There are two ways to create any (every?) collection of bytes: [[memory|heap-allocation]] and [[memory|stack-allocation]].[^0]

## Types

Rust has two types of string variables: `String` and `&str` (string slice).

### `String`
Allocated on the [[memory|heap]]. Heap-allocated variables are mutable (i.e. size can change), which means: _`String` variables retain [[ownership]] over their address in memory._

Similar to a vector i.e. a 1-dimensional array. Like arrays you can append to them (`push()`), remove segments of them (`pop()`).

Has its own [[buffer]] in memory: that is, it has [[rust-ownership-borrowing-system|ownership]] of the memory where its bytes are stored.

### `&str`
A _string slice_: think of it as a [[pointer]] to _another_ string (set of bytes) that's actually owned by another variable. Also called a [[rust-ownership-borrowing-system|borrowed reference]]. Because `&str` types are referencing something else, they are immutable. Can also think of it this way: you wouldn't alter a dress you borrowed from a friend.

### string literals
? Mentioned but not defined. `&str` slices from these too, not just `String`.

Static string. Rust compiles all string literals into static string slices. These exist in the binary code of the executable and are immutable.

## Use cases
Use `String` when you want to build a string dynamically. Example:
>in our markdown compiler, we will be using `String`s to hold the value of each block of HTML code; if we were going to write `<h1>Hello, world!</h1>`, we would `push()` the first tag, then the inner content, then the closing tag.





[^0]: [[memory|Heap-allocated]] variables are dynamically created at [[program lifecycle|runtime]]. [[memory|Stack-allocated]] variables are assigned at [[program lifecycle|compile time]].
