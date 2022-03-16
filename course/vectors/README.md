# Table of Contents📚
- [What is a vector❔](#what-is-a-vector)
- [Declaring a vector](#declaring-a-vector)
- [Declaring a vector with elements](#declaring-a-vector-with-elements)
- [Accessing elements](#accessing-elements)
- [Joining elements](#joining-elements)
- [Pushing elements](#pushing-elements)
- [Removing elements](#removing-elements)

# Vectors
## What is a vector❔
A vector is a data structure that can store a collection of data of the same type.

## Declaring a vector
To declare an empty vector, use the `Vec<T>` type, where `T` is the type of the elements in the vector.
```rust
let mut string_vec: Vec<String> = Vec::new();
```
> ℹ️ We have to make the vector mutable to be able change its elements.

> ℹ️ We use the `Vec::new()` method to create an empty vector.


## Declaring a vector with elements
Declaring a vector with default values is much easier.
And we don't need to specify the type of the elements.
```rust
let mut string_vec = vec!["Hello", "World"];
```
> ℹ️ We use the `vec!` macro to create a vector with the given elements.


## Accessing elements
```rust
let mut string_vec = vec!["Hello", "World"];
println!("{} 👋", string_vec[0]);
```
> ℹ️ We use the `[]` operator to access the element at the given index.

Output:
```
Hello 👋
```

## Joining elements
To join the elements of a vector with a specific separator, we can use the `join` method.
```rust
let mut string_vec = vec!["Hello", "World"];
println!("{}", string_vec.join("!"));
println!("{}", string_vec.join("->"));
println!("{}", string_vec.join(" "));
```

Output:
```
Hello!World
Hello->World
Hello World
```

## Pushing elements
We can push elements to the end of the vector using the `push` method.
```rust
let mut string_vec = vec!["I", "Love"];

string_vec.push("Rust");

println!("{} 💖", string_vec.join(" "));
```
Output:
```
I Love Rust 💖
```
## Removing elements
We can remove an element with its index using the `remove` method.
```rust
let mut string_vec = vec!["I", "Love", "Rust"];

string_vec.remove(1);

println!("{} 💖", string_vec.join(" "));
```
Output:
```
I Rust 💖
```


---

<p align="right"><a href="../reading-a-file">Next Section ⏭️</a></p>


---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>