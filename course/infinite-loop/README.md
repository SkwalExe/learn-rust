# Table of Contents📚
- [the loop keyword♾️](#the-loop-keyword)
- [the break keyword🛑](#the-break-keyword)
- [the continue keyword➡️](#the-continue-keyword)

# Infinite loop♾️
## the loop keyword♾️
Loops allow us to execute a block of code infinitely until we specify when to stop it.
For example, we can use the `loop` keyword to print hello infinitely.
```rust
loop {
    println!("Hello");
}
```
Output:
```
Hello
Hello
Hello
Hello
Hello
Hello
Hello
...
```
## the break keyword🛑
The `break` keyword allows us to stop the execution of a loop.
Imagine that we want to print hello 5 times, and then stop the execution of the loop.
```rust
let mut count = 0;

loop {
    println!("Hello");
    count = count + 1;

    if count == 5 {
        break;
    }
}
```
We add 1 to the variable `count` each time we print hello, and then when `count` is equal to 5, we stop the execution of the loop.

Output:
```
Hello
Hello
Hello
Hello
Hello
```
## the continue keyword➡️
The `continue` keyword allows us to skip the current iteration of the loop and continue with the next one.
> ℹ️ an iteration is a single execution of the loop body.
Imagine that we want to print hello 5 times, but we want to skip the second one.
```rust
let mut count = 0;

loop {
    count += 1;

    if count == 2 {
        continue;
    }

    println!("{} : Hello", count);

    if count == 5 {
        break;
    }
}
```

> ℹ️ `count += 1` is the same as `count = count + 1`

We add 1 to the variable `count` each time we print hello, and then when `count` is equal to 2, we skip the current iteration and continue with the next one.

Output:
```
1 : Hello
3 : Hello
4 : Hello
5 : Hello
```

---

<p align="right"><a href="https://github.com/SkwalExe/learn-rust/tree/main/course/while-loop">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>