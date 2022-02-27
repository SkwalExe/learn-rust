# Table of contents📚
- [What is a reference ❔](#what-is-a-reference)
- [How to create a reference ❔](#how-to-create-a-reference)
- [How to use a reference 🤹](#how-to-use-a-reference)
- [Modifying a reference ✏️](#modifying-a-reference)
    - [Firstly](#firstly)
    - [Secondly](#secondly)
- [Warning ⚠️](#warning)
    - [Firstly](#firstly)
    - [Secondly](#secondly)

# References🔗
## What is a reference❔
A reference is just another way to refer to a variable, it is similar to a pointer in other languages.

For exampe if your 🐕 Dog is called `Domenic`, and you call him `Dom`, you're still referring to him. So `Dom` is a reference to `Domenic`.



```
Dom ----------> Domenic
                🐕 Your dog
```

This is the same with variables.



## How to create a reference❔
First, we need to create a variable.
```rust
let domenic = "Dog 🐶";
```
Then, we can create a reference to the variable by adding the `&` symbol before the variable name.
```rust
let mut dom = &domenic;
```
The `&` symbol means that we want to get a reference to the variable next to it.

So now, the variable `Dom` is a reference to `Domenic`.

## How to use a reference🤹
You can use a reference to access the value of the variable.
For example, if you want to print the value of the variable `dom`, you can do it like this:
```rust
println!("The value of Dom is : {}", dom);
println!("The value of Domenic is : {}", domenic);
```
The output will be:
```
The value of Dom is : Dog 🐶
The value of Domenic is : Dog 🐶
```

> ℹ️ We can have multiple references to the same variable.

## Modifying a reference✏️
`dom` being a reference to `Domenic`, it looks like we can modify it's value by doing 
```rust
dom = "Doggo 🐶";
```
But this is not possible.
### Firstly
Because by defaults, references are immutable, so we can't modify the value of the variable.

To make a reference mutable, we need to add the `mut` keyword before the variable name.

```rust
let dom = &mut domenic;
```
Now, we can modify the value of the variable.

### Secondly
When we do 
```rust
dom = "Doggo 🐶";
```
We don't modify the value of the variable `Domenic`, but we modify the value of the variable `Dom` that is a reference to `Domenic`.

#### **Before**
```
Dom             Domenic
--------------> "Dog 🐶"
```
#### **After**
```
Dom            Domenic
"Doggo 🐶"     "Dog 🐶"
```

To modify the value of the variable `Domenic`, we need to use the `*` symbol before the variable name.
```rust
*dom = "Doggo 🐶";
```

Because `*dom` means that we are referring to the **value** of `domenic` not the value of `dom`.

## Warning⚠️
### Firstly
We can't have more than one mutable reference to the same variable.
### Secondly
You can only use one mutable reference at the same time depending on the rustc version.

In the following example : 
```rust
let mut username = "Super cool username 💪";
let username_ref = &mut username;

println!("The username is : {}", username);
```

We will encounter an error because the `println!` macro borrows the variable `username` and we already have a mutable reference to it.

---

<p align="right"><a href="https://github.com/SkwalExe/learn-rust/tree/main/course/structs">Next Section ⏭️</a></p>


---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>