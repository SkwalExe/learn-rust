# Table of contents📚

- [What is a trait❔](#what-is-a-trait)
- [Implementing a trait](#implementing-a-trait)
- [Using traits](#using-traits)

# Implementing traits

## What is a trait❔

A trait is a set of methods common to each type. 
It is similar to an interface in other languages.

## Implementing a trait

First, we need a struct to implement the trait on :

```rust
struct Person {
    name: String,
    age: u8,
    hobbies: Vec<String>,
    country: String,
    company: String,
}
```

We will implement the `to_string` trait for the `Person` struct.

This method will return a string representation of the instance of the struct.

To implement a trait, we need to use the `impl` keyword and the following syntax:

```rust
impl ToString for Person {
    fn to_string(&self) -> String {
        format!("Hi, my name is {}, I'm {} years old and I live in {}. I work at {} and my hobbies are: {}", self.name, self.age, self.country, self.company , self.hobbies.join(", "))
    }
}
```

> ℹ️ The `format!` macro is used like `println!` but it returns a `String` instead of printing to the console.

## Using traits

We can now create a new instance of the struct and use the `to_string` method:

```rust
let person = Person {
    name: String::from("Léopold"),
    age: 13,
    hobbies: vec![String::from("💻"), String::from("🛌"), String::from("🍔")],
    country: String::from("France 🇫🇷"),
    company: String::from("Skwal-net"),
};

let presentation = person.to_string();

println!("{}", presentation);
```

> ℹ️ The traits name are the same for all types.

Output:

```
Hi, my name is Léopold, I'm 13 years old and I live in France 🇫🇷. I work at Skwal-net and my hobbies are: 💻, 🛌, 🍔
```

---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home 🏠</a> - <a href="../vectors">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>