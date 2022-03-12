# Table of Contents📚
- [What are data types❓](#what-are-data-types)
- [Specifying data types](#specifying-data-types)

# Variable data types 
## What are data types❓
When we declare a variable, for example :
```rust
let x = 5;
```
The value of `x` is `5`, and `5` is, of course, a number. But more precisely, `5` is of type `i32`, which means its an 32-bit signed integer.

> ℹ️ An unsigned integer is an integer that is always positive, whereas a signed integer is an integer that can be positive or negative.

There are many other data types in Rust. 
```
i8, i16...  -> signed integers 🔢 
u8, u16...  -> unsigned integers 🔢 
f32, f64    -> floating point numbers 🔢 
char        -> a single character 🔤
bool        -> either true or false 👍👎
String      -> a sequence of characters ✍️
```

## Specifying data types
 
When we declare a variable, we don't need to specify its type like in other languages like Java or C, because Rust is an `autotyped` language, which means that rust will automatically determine the type of the variable.

But, if we want to specify the type of the variable, we can do it with the following syntax:
```rust
let x: type = value;
```
for example:
```rust
let x: i32 = 5;
```

You should always specify the type of the variable, because it is a good practice to avoid errors.

for example, if you know that `x` will never be negative, you can write:
```rust
let x: u32 = 1;
```

*And that's how we manipulate variable data types!*





---

<p align="right"><a href="../if-else-statements">Next Section ⏭️</a></p>


---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>