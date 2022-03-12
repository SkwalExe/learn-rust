# Table of contents📚
- [What is a tuple struct❔](#what-is-a-tuple-struct)
- [How to create a tuple struct❔](#how-to-create-a-tuple-struct)
- [How to use a tuple struct🤹](#how-to-use-a-tuple-struct)
- [Modifying a tuple struct✏️](#modifying-a-tuple-struct️)


# Tuple structs🧱
## What is a tuple struct❔
Tuple structs are similar to structs, but they are used to group data together in a tuple, and without a name for the fields.
## How to create a tuple struct❔
We can create a tuple struct by using the keyword `struct` and then the name of the struct capitalized, followed by a tuple of the data types of the fields.
```rust
struct Color(u8, u8, u8);
//           r   g   b
```
## How to use a tuple struct🤹
We can create an instance of the tuple struct with the following syntax:
```rust
let black = Color(0, 0, 0);
```
We can access the values of the tuple struct by using the dot operator and the index `struct.index` :
```rust
println!("🟥 Red value : {}", black.0);
println!("🟩 Green value : {}", black.1);
println!("🟦 Blue value : {}", black.2);
```
Output:
```
🟥 Red value : 0
🟩 Green value : 0
🟦 Blue value : 0
```
## Modifying a tuple struct✏️
By default, like variables, tuple structs are immutable.
So we have to make them mutable by adding the `mut` keyword before the struct name when creating an instance of it.
```rust
// declaring an instance of the tuple struct
let mut black = Color(0, 0, 0);
// modifying the value of the first field
black.0 = 255;
```


---

<p align="right"><a href="../pass-by-reference">Next Section ⏭️</a></p>


---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>