# Table of contents📚
- [The `use` keyword](#the-use-keyword)
- [The `open` and `expect` methods](#the-open-and-expect-methods)
- [The `read_to_string` method](#the-read_to_string-method)

# Reading a file📖
## The `use` keyword
First, we need a file to read, so we will create a new file in our project folder.
```bash 
# 📄 hello.txt
World, Hello 👋
```
Now, we will read the file and print its content.

First, we need to import the `File` struct from the `std::fs` module, which is the standard library for file handling.
To import a module, we use the `use` keyword.
```rust
use std::fs::File;
```
Then we need to import `std::io::prelude::*;` to allow us to perform read and write operations on the file.
```rust
use std::io::prelude::*;
```
The `*` means that we are importing all the methods from the prelude module.

## The `open` and `expect` methods 
The `open` method returns a `Result` type, which is a type that represents either a value or an error.
We can use the `expect` method to unwrap the `Result` type and get the value.
The value is a variable of type `File`.
The `open` method takes a path to the file as an argument.
```rust
let mut file = File::open("hello.txt").expect("Unable to open file");
```
The `expect` method is used to handle errors, if the file cannot be opened for any reason, the program will `panic`. For exemple if the file doesn't exist, the program will print the error message and exit.
```
thread 'main' panicked at 'Failed to open hello.txt: Os { code: 2, kind: NotFound, message: "No such file or directory" }', rust.rs:5:41
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
```

## The `read_to_string` method
the `read_to_string` takes a mutable reference to a `String` as an argument and returns a `Result` type. This function will read the entire file and store it in the `String` variable.
```rust
let mut contents = String::new();
file.read_to_string(&mut contents).expect("Unable to read file");

println!("📄 file content : {}", contents);
```
Output:
```
📄 file content : World, Hello 👋
```


<!--
---

<p align="right"><a href="../reading-a-file">Next Section ⏭️</a></p>
-->

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>