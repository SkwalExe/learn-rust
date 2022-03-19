# Table of Contents📚

- [What is a function❓](#what-is-a-function)
- [Declaring a function](#declaring-a-function)
- [Returning values](#returning-values)

# Functions🛠️

## What is a function❓

A function is a block of code that takes an input and produces an output.

## Declaring a function

A function can be declared with the `fn` keyword.

> ℹ️ Functions have to be declared outside of the main function and before they are called.

```rust
fn function_name(param1: Type, param2: Type) {
    // function body
}
```

Exemple, write a function called `hello` that says `🔔 TIME TO EAAT` x times:

```rust
fn hello(x: i32) {
    for _ in 0..x {
        println!("🔔 TIME TO EAAT");
    }
}

fn main() {
    hello(5);
}
```

Output:

```
🔔 TIME TO EAAT
🔔 TIME TO EAAT
🔔 TIME TO EAAT
🔔 TIME TO EAAT
🔔 TIME TO EAAT
```

## Returning values

Functions can return a value with the `return` keyword.

For example, create a function `isEven` that returns true or false depending on whether the input is even or odd:

```rust
fn is_even(x: i32) -> bool {
   return x % 2 == 0
}
```

> ℹ️ We **have to** specify the return type of a function with the `->`  after the function name and parameters.

The `%` operator is called the modulo operator. It returns the remainder of an euclidean division.
So if we have a number `x` and we want to know if it is even, we can use the modulo operator to check if the ramainder of its euclidiand division by 2 is 0.

We can now use the `isEven` function to print even numbers from 1 to 10:

```rust
fn main() {
    for i in 1..11 {
        if is_even(i) {
            println!("{} is even", i);
        }
    }
}
```

Output:

```
2 is even
4 is even
6 is even
8 is even
10 is even
```

---

<p align="right"><a href="../code-blocks">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>