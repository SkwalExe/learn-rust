# Table of Contents📚
- [What is a struct method❔](#what-is-a-struct-method)
- [The `impl` keyword](#the-impl-keyword)
- [Multiple methods](#multiple-methods)

# Struct methods🛠️
## What is a struct method❔
Structs methods are functions that are attached to structs, to make them easier to use.
## The `impl` keyword
If we have a struct named `Person`
```rust
struct Person {
    name: String,
    age: u8,
    hobbies: Vec<String>,
    country: String,
    company: String,
}
```
> ℹ️ `hobbies` is a vector of strings.

We can create a method for the struct that will introduce the person.

To declare methods for a struct, we use the `impl` keyword, like this:
```rust
impl Person {
    fn introduce(&self) {
        println!("Hi, my name is {}, I'm {} years old and I live in {}. I work at {} and my hobbies are: {}", self.name, self.age, self.country, self.company , self.hobbies.join(", "));
    }
}
```
> ℹ️ The function takes the `&self` parameter, that corresponds to the struct instance that we want to use the method on.

> ℹ️ The join method is a method that joins the items of a vector with a separator to create a string.

We can now create a new instance of the struct and use the method.
```rust
fn main() {
    let person = Person {
        name: String::from("Léopold"),
        age: 13,
        hobbies: vec![String::from("💻"), String::from("🛌"), String::from("🍔")],
        country: String::from("France 🇫🇷"),
        company: String::from("Skwal-net"),
    };

    person.introduce();
}
```
> ℹ️ The `String::from` is a function that creates a `String` from a string literal. `str` and `String` are different types, but they are both used to represent strings.
Output:
```
Hi, my name is Léopold, I'm 13 years old and I live in France 🇫🇷. I work at Skwal-net and my hobbies are: 💻, 🛌, 🍔
```

## Multiple methods
We can also create multiple methods for a struct.

let's add a method `is_adult` to the struct `Person`:
```rust
impl Person {
    fn introduce(&self) {
        ...
    }

    fn is_adult(&self) -> bool {
        self.age >= 18
    }
}
```
> ℹ️ the `is_adult` doesn't need the `return` keyword, because when a method returns a value, it returns the value of the last expression.

We can now use the method `is_adult` on the instance of the struct.
```rust
fn main() {
    let person = Person {
       ...
    };

    if person.is_adult() {
        println!("{} is an adult ✅", person.name);
    } else ❔{
        println!("{} is not an adult ⛔", person.name);
    }
}
```
Output:
```
Léopold is not an adult ⛔
```

<!--
---

<p align="right"><a href="https://github.com/SkwalExe/learn-rust/tree/main/course/impl-keyword">Next Section ⏭️</a></p>
-->

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>