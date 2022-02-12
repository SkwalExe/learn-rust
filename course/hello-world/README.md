# Hello world 
## Writing the program
We will start this course by creating an hello world program with the rust programming language.

We will start by creating a new folder `hello-world` and a file `main.rs` inside it.

> `.rs` is the extension for rust files.

We can now open the file `main.rs` in our IDE, as well as a terminal of your choice, and start writing our program.

We declare a function called `main` because all rust programs begin with a function `main`.

```rust
// main.rs
fn main() {

}
```

> the `fn` keyword is used to declare a function.

> the lines starting with `//` are comments, they are ignored when executing the program.

In the function, we will call the `println!` macro to print a message to the console. And we pass the string `Hello, world!` as an argument.

```rust
// main.rs
fn main() {
    println!("Hello, world!");
}
```

> All instructions end with a semicolon `;`
## Running the program
Now that we have coded our program, we will compile it and run it.

to compile the program, we can use the `rustc` command.

```bash
$ rustc main.rs
```

Running this command created an executable file called `main` in the current directory that we can run by typing `./main`.

```bash
$ ./main
> Hello, world!
```

*And that's how we write an hello world program in rust !*

<p style="text-align: right">
    <a href="https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world-cargo/">Next Section</a>
</p>

---

<p style="text-align: right">
    Course created by <a href="https://github.com/SkwalExe/">Skwal</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL">Dcode</a>
</p>
