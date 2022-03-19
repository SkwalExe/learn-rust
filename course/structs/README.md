# Table of contents📚

- [What is a struct❔](#what-is-a-struct)
- [How to create a struct❔](#how-to-create-a-struct)
- [How to use a struct🤹](#how-to-use-a-struct)
- [Modifying a struct✏️](#modifying-a-struct️)

# Structs🧱

## What is a struct❔

Structs are a way to group related data together in a data type.

## How to create a struct❔

We know that an user can have a username, and an email.

So we can create a struct to represent this data instead of having two variables.

To create a struct, we use the keyword `struct` and then the name of the struct capitalized.

```rust
struct User {
    username: str,
    email: str,
}
```

> ℹ️ structs are declared outside the main function.

> ℹ️ We have to specify the type of the  variables inside the struct.

## How to use a struct🤹

Now that we have a struct we can create an `instance` of it.

Imagine having an user with the username `Bob 🐡` and the email `bobthefish@skwal.net`.

```rust
let bob = User {
    username: "Bob 🐡",
    email: "bobthefish@gmail.com",
};
```

We can access the values of the struct by using the dot operator `struct.field` : 

```rust
println!("Hello, {} ! We sent you an email at {}", bob.username, bob.email);
```

Output:

```
Hello, Bob 🐡 ! We sent you an email at bobthefish@skwal.net
```

## Modifying a struct✏️

By default, like variables, structs are immutable.

So we have to make them mutable by adding the `mut` keyword before the struct name when creating an instance of it.

```rust
let mut bob = User {
    username: "Bob 🐡",
    email: "bobthefish@gmail.com",
};

bob.username = "Bob 2.0 🐠";

println!("New username : {}", bob.username);
```

Output:

```
New username : Bob 2.0 🐠
```

---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home 🏠</a> - <a href="../tuple-structs">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>