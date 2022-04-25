# Table of contents📚

- [Creating a file 📝](#creating-a-file-)
- [Writing to a file 📝](#writing-to-a-file-)

# Writing to a file 📝

## Creating a file 📝

First, we need to import some modules to execute operations on files.

```rust
use std::fs::File;
use std::io::prelude::*;
```

To create a file, we will use the `File::create` method.

```rust
let mut file = File::create("hello.txt").expect("Unable to create file");
```

We specify the name of the file as the first argument.

Now, let's try to run the program.

```bash
$ cargo run
```

We can now see, in the root of the project, a file called `hello.txt`.

## Writing to a file 📝

Let's write some text to the file.

For this, we will use the `write_all` method.

```rust
file.write_all(b"Hello world!").expect("Unable to write to file");
```

The program ignore if a file already exists when creating it.

Inside the `write_all` method, we add a `b` before the string to convert it to a byte array because the `write_all` method only accepts byte arrays.

The `write_all` method will overwrite the content of the file.

Now if we run the program again, we can see that the file contains the text `Hello world!`.

---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home 🏠</a> - <a href="../defining-traits">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>