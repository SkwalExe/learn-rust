# Table of Contents📚
- [What is a for loop❓](#what-is-a-for-loop)
- [The for keyword🔑](#the-for-keyword)
- [Vector iteration](#vector-iteration)
  - [What is a vector❓](#what-is-a-vector)
  - [Declaring a vector](#declaring-a-vector)
  - [Iterating over a vector](#iterating-over-a-vector)
  - [Iterating over a vector with index🔢](#iterating-over-a-vector-with-index)


# For loops🔢
## What is a for loop❓
For loops are used to iterate over a given sequence.

## The for keyword🔑
The `for` keyword is used to create a for loop.

Example:

```rust
for count in 0..5 {
    println!("🔢 -> {}", count);
}
```
Here, `count` is the variable that holds the current value of the loop, and `0..5` is an expression that generates the range of values to iterate over. 

`0..5` is the range of values from 0 to 5 (5 not included).

Output:
```
🔢 -> 0
🔢 -> 1
🔢 -> 2
🔢 -> 3
🔢 -> 4
```

**It is possible to store a range in a variable:**
```rust
let range = 0..5;
for count in range {
    println!("📢 {}", count);
}
```
Output:
```
📢 0
📢 1
📢 2
📢 3
📢 4
```
## Vector iteration
### What is a vector❓
A vector is a group of values that can be iterated over.
### Declaring a vector
A vector can be declared with the `vec!` macro and the values separated by commas.
Example:
```rust
let animals = vec!["🐒 Monkey", "🐕 Dog", "🦄 Unicorn"];
```
### Iterating over a vector
A vector can be iterated over using the `for` loop.

Example:
```rust
let animals = vec!["🐒 Monkey", "🐕 Dog", "🦄 Unicorn"];

for animal in animals.iter() {
    println!("My 💫 favorite animal 💫 is the {}", animal);
}
```
Output:
```
My 💫 favorite animal 💫 is the 🐒 Monkey
My 💫 favorite animal 💫 is the 🐕 Dog
My 💫 favorite animal 💫 is the 🦄 Unicorn
```
> ℹ️ We use the `iter()` method to get an iterator over the vector and to prevent the ownership of the vector from being moved and being able to use it after the loop 

### Iterating over a vector with index🔢
It is possible to iterate over a vector knowing the index of the current element.

We can do that with the `enumerate()` method.

Example:

```rust
let fruits = vec!["🍇 Grapes", "🍈 Melons", "🍌 Bananas"];

for (index, fruit) in fruits.iter().enumerate() {
    println!("I love {} at index {}", fruit, index);
}
```
Output:
```
I love 🍇 Grapes at index 0 
I love 🍈 Melons at index 1
I love 🍌 Bananas at index 2
```
> ℹ️ We use `(index, number)` because the `enumerate()` method returns a tuple with the index and the value.




---

<p align="right"><a href="../enum-types">Next Section ⏭️</a></p>


---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>