# Table of Contents📚
- [What is shadowing❓](#what-is-shadowing)
- [Usage](#usage)


# Shadowing👥
## What is a shadowing❓
When we modify a variable inside a code block, the change will remain outside it, but it is possible to make the variable back to its original value when the code block ends. This is called shadowing.

## Usage
For example, we can use a code block to modify a variable:
```rust
let worm_name = "Wormie 🪱";

{
    worm_name = "Wormy 🪱";
    println!("My Worm is called {}", worm_name);
}

println!("My Worm is called {}", worm_name);
```
Output:
```
My Worm is called Wormy 🪱
My Worm is called Wormy 🪱
```

We can see that the change of the variable `worm_name` is still available outside the code block. We can shadow the variable with a new one inside the code block by adding the `let` keyword before the variable name.

```rust
let worm_name = "Wormie 🪱";

{
    let worm_name = "Wormy 🪱";
    println!("My Worm is called {}", worm_name);
}

println!("My Worm is called {}", worm_name);
```
Output:
```
My Worm is called Wormie 🪱
My Worm is called Wormy 🪱
```


<!--
---

<p align="right"><a href="https://github.com/SkwalExe/learn-rust/tree/main/course/shadowing">Next Section ⏭️</a></p>
-->

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>