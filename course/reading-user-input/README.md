# Reading user input ⌨️

To read user input from the command line, we will use the standard `io` module

```rust
use std::io;
```

Now, we need a variable to store the user input.

```rust
let mut input = String::new();
```

And we need to print something to ask the user for input.

```rust
println!("Please enter your name: ");
```

Finally, we need to read the user input with the `stdin().read_line()` method.

```rust
io::stdin().read_line(&mut input);
// we give the read_line function a mutable reference to our input variable
```

The `read_line` function returns a `Result` type, which is a type that can either be `Ok` or `Err`.

So, we will put this in a `match` expression.

```rust
match io::stdin().read_line(&mut input) {
    Ok(_) => println!("Hello {}", input),
    Err(error) => println!("Error: {}", error),
}
```

We put a `_` in the Ok branch because we don't care about the value of the `Result` (which is the numeber of bytes that were written to the buffer).

Now, we can run the program.

```bash
> cargo run
Please enter your name:
> John
Hello John
```

<!--
---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home 🏠</a> - <a href="../defining-traits">Next Section ⏭️</a></p>
-->

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>