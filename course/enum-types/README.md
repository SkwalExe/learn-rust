# Table of Contents📚
- [What is an enum type ❓](#what-is-an-enum-type)
- [Declaring an enum type](#declaring-an-enum-type)
- [Matching on an enum](#matching-on-an-enum)
    - [What is a match expression ❓](#what-is-a-match-expression)
    - [Usage](#usage)
    - [Matching on an enum](#matching-on-an-enum)
    

# Enum types
## What is an enum type❓
Enums are a way to express your code in a descriptive and simple way.
They are a way to group related values together.
## Declaring an enum type
An enum can be declared with the `enum` keyword, followed by the name of the enum, and then a list of variants.
> ℹ️ **The enums have to be declared out of the main function.**

Example:
```rust
enum Animal {
    Monkey,
    Dog,
    Unicorn,
}

fn main() {
    ///
}
```
> ℹ️ The enum and variants name are conventionally capitalized.

We can now use the enum to create a variable of type `Animal`.
```rust
let animal:Animal = Animal::Monkey;
```
> ℹ️ We can use the `::` operator to specify the variant of the enum (`Monkey` in this case).

## Matching on an enum
### What is a match expression❓
The `match` keyword is used to do different thingd based on the value of a variable.
> ℹ️ It is similar to switch statements in other languages.

### Usage
```rust
match variable {
    value => {
        // Do something
    }
    value2 => {
        // Do something else
    }
    _ => {
        // Do something else
    }
}
``` 
> ℹ️ We can ignore the `{}` if wa expect only one line of code.

> ℹ️ The `_` is a catch all case that is used when no other cases match.
### Matching on an enum
We can use the `match` keyword to match on an enum.
```rust
match animal {
    Animal::Monkey => println!("🐒"),
    Animal::Dog => println!("🐶"),
    Animal::Unicorn => println!("🦄"),
    _ => println!("🤖"),
}
```
| value             | Output |
| ----------------- | ------ |
| `Animal::Monkey`  | 🐒      |
| `Animal::Dog`     | 🐶      |
| `Animal::Unicorn` | 🦄      |
| Other             | 🤖      |


---

<p align="right"><a href="../constants">Next Section ⏭️</a></p>


---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>