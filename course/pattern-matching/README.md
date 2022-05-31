# Table of Contents📚

- [The `match` keyword](#the-match-keyword)
- [Multiple patterns](#multiple-patterns)
- [Checking if a value is in a range](#checking-if-a-value-is-in-a-range)

# Pattern matching 🔍

## The `match` keyword

The `match` keyword is similar the the `switch` keyword in other languages.

It is a conditional operator, it is used to do different things based on the value of a variable.

for example:

```rust
let number = 2;

match number {
    1 => println!("the number is 1"),
    2 => println!("the number is two"),
    3 => {
        println!("the number is 3");
        println!("the number is 3 again");
      },
    _ => println!("the number is not one, two or three")
}
```

the `_` is the wildcard, it will be used if no other match is found.

You must add `{}` if you want to execute multiple lines of code on a match.

The checked value and all the patterns must be of the same type.

Now if we run the program : 

```bash
$ cargo run
> the number is two
```

## Multiple patterns

You can check multiple patterns at the same time with a `|`

```rust
let number = 3;

match number { 
    1 | 3 => println!("the number is 1 or 3"),
    _ => println!("the number is not one or three")
}
```

```bash
$ cargo run
> the number is 1 or 3
```

## Checking if a value is in a range

We can also check if a number is in a range.

```rust
let number = 4;

match number { 
    1...5 => println!("the number is between 1 and 5"),
    _ => println!("the number is not between 1 and 5")
}
```

If we run the program : 

```bash
$ cargo run
> the number is between 1 and 5
```





---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home 🏠</a> - <a href="../reading-user-input">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>