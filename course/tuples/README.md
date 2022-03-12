# Table of Contents📚
- [What is a tuple❓](#what-is-a-tuple)
- [Declaring a tuple](#declaring-a-tuple)
- [Accessing a tuple](#accessing-a-tuple)
- [Extracting values from a tuple🚪](#extracting-values-from-a-tuple)

# Tuples
## What is a tuple❓
A tuple is a collection of values that can be of different types.
> ℹ️ Tuples are usually used to return multiple values from a function.

> ℹ️ Tuples can contain other tuples.
## Declaring a tuple
A tuple can be declared with the following syntax:
```rust
let zoo = ("🦍 Gorilla", "🦊 Fox", "🦓 Zebra", "🐘 Elephant");
```
## Accessing a tuple
We can access different values in a tuple with the following syntax: `tuple.index`

Example, print the first value in the tuple:
```rust
let zoo = ("🦍 Gorilla", "🦊 Fox", "🦓 Zebra", "🐘 Elephant");

println!("The first animal in the zoo is the ", zoo.0);
```
Output:
```
The first animal in the zoo is the 🦍 Gorilla
```
## Extracting values from a tuple🚪
We can extract values from a tuple and store them in variables with the following syntax: 
```rust
let zoo = ("🦍 Gorilla", "🦊 Fox", "🦓 Zebra", "🐘 Elephant");

let (a, b, c, d) = zoo;

println!("In the zoo, there is a {}, a {}, a {}, and an {}", a, b, c, d);
```
Output:
```
In the zoo, there is a 🦍 Gorilla, a 🦊 Fox, a 🦓 Zebra, and an 🐘 Elephant
```



---

<p align="right"><a href="../functions">Next Section ⏭️</a></p>


---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>