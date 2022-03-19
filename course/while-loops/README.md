# Table of Contents📚

- [What is a while loop❓](#what-is-a-while-loop)
- [The while keyword🔁](#the-while-keyword)
- [The break and continue keywords🔑](#the-break-and-continue-keywords)

# While loops🔁

## What is a while loop❓

While loop are used to execute a block of code as long as a condition is true.

## The while keyword🔁

The `while` keyword is used to create a while loop. 

Example:

```rust
let mut cats = 0;

while count < 5 {
    println!("There are {} cats 🐈", count);

    // Increment `count`
    count += 1;
}
```

While `cats` is less than 5, we will print the value of `cats` on a new line, and then increment `cats` by 1.

Output:

```
There are 0 cats 🐈
There are 1 cats 🐈
There are 2 cats 🐈
There are 3 cats 🐈
There are 4 cats 🐈
```

## The break and continue keywords🔑

We can also use the `break` and `continue` keywords as seen in the [Infinite Loop ♾️ Section](https://github.com/SkwalExe/learn-rust/tree/main/course/infinite-loop).

---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home 🏠</a> - <a href="../for-loops">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>