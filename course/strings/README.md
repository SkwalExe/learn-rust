# Table of Contents📚
- [What is a string❔](#what-is-a-string)
- [`len` method](#len-method)
- [`is_empty` method](#is_empty-method)
- [`split_whitespace` method](#split_whitespace-method)
- [`contains` method](#contains-method)
- [`push_str` method](#push_str-method)


# Strings📝
## What is a string❔
In programming, a string is a sequence of characters.
In rust, there are two datatypes types for strings: `str` and `String`.

`str` is the primitive type that represents a string, `String` is more powerful.

In this section, we will be referring to the type `String`. 

## `len` method
The `len` method is used to get the length of a string, it returns an `usize` value.
```rust
let name = String::from("Léopold");

println!("My name has {} characters", name.len());
```
Output:
```
My name has 8 characters
```
## `is_empty` method
The `is_empty` method is used to check if a string is empty, it returns a `bool` value.
```rust
let name = String::from("Léopold");
let empty = String::from("");

if name.is_empty() { // check if name is an empty string
    println!("'{}' is empty", name);
} else {
    println!("'{}' is not empty", name);
}

if empty.is_empty() { // check if empty is an empty string
    println!("'{}' is empty", empty);
} else {
    println!("'{}' is not empty", empty);
}
```
Output:
```
'Léopold' is not empty
'' is empty
```
## `split_whitespace` method
The `split_whitespace` method is used to split a string into substrings, it returns an iterator so we can iterate over the substrings.
```rust
let text = String::from("Hello world");

for word in text.split_whitespace() {
    println!("Word : {}", word);
}
```
Output:
```
Word : Hello
Word : world
```
## `contains` method
The `contains` method is used to check if a string contains a substring, it returns a `bool` value.
```rust
let text = String::from("Hello world");

if text.contains("world") {
    println!("'{}' contains 'world' ✅", text);
} else {
    println!("'{}' does not contain 'world' ⛔", text);
}
```
Output:
```
'Hello world' contains 'world' ✅
```
## `push_str` method
The `push_str` method is used to happend text to a string, the string needs to be mutable because we are changing it.
```rust
let mut text = String::from("Hello"); 

println!("{}", text); 

text.push_str(" world"); 

println!("{}", text);
```
Output:
```
Hello
Hello world
```






---

<p align="right"><a href="https://github.com/SkwalExe/learn-rust/tree/main/course/implementing-traits">Next Section ⏭️</a></p>


---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>