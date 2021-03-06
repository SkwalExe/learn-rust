# Table of Contentsπ

- [What is cargoβ](#what-is-cargo)
- [Creating a new projectπ](#creating-a-new-project)
- [Compiling and running a program with cargoπ](#compiling-and-running-a-program-with-cargo)
  - [Just compiling](#just-compiling)
  - [Compiling and runningπ](#compiling-and-running)

# Hello world with cargoπ’

## What is cargoβ

Cargo is a **Rust package manager**. It is used to manage dependencies and build Rust projects.

## Creating a new projectπ

We will create a new project called `hello-world-cargo`, to do this, we will use the following command.

> βΉοΈ the `--bin` parameter flags the project as an application, not a library.

```bash
$ cargo new hello-world-cargo --bin

> Created binary (application) `hello-world-cargo` package.
```

This command created a new folder `π hello-world-cargo` in the current directory.

This folder contains a `π Cargo.toml` file, a `π src` folder and a `π main.rs` file.

```bash
hello-world-cargo
βββ Cargo.toml
βββ .git
β   βββ ...
βββ .gitignore
βββ src
    βββ main.rs
```

It also initialized a git repository for the project.

The `π src` folder contains the source code of the application, in it there already is a `π main.rs` file containing an hello world program.

```rust
// π main.rs
fn main() {
    println!("Hello, world π");
}
```

| File           | Description                                                                                              |
| -------------- | -------------------------------------------------------------------------------------------------------- |
| `π Cargo.toml` | The Cargo manifest file, this file contains all the dependencies and the application name.               |
| `π src`        | The source folder, this folder contains the source code of the application.                              |
| `π main.rs`    | The main file, this file contains the source code of the application.                                    |
| `π .git`       | The git folder, this folder contains all the git files, you can ignore this folder if you don't use git. |
| `π .gitignore` | The git ignore file, this file contains all the files that should be ignored when committing.            |

## Compiling and running a program with cargoπ

### Just compiling

To compile the program, we will use the `cargo build` command.

```bash
# hello-world-cargo π
$ cargo build
```

This command will compile the program and create an executable file called `π hello-world-cargo` in the new `π target/debug` folder.

```bash
# hello-world-cargo/target/debug π
$ ./hello-world-cargo
> Hello, world π
```

![](1.png)

### Compiling and runningπ

To compile and run the program, we will use the `cargo run` command.

```bash
# hello-world-cargo π
$ cargo run
...
> Hello, world π
```

![](2.png)

---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home π </a> - <a href="../variables">Next Section β­οΈ</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>