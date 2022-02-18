# Table of Contents📚
- [Declaring a variable](#declaring-a-variable)
- [Printing a variable💬](#printing-a-variable)
- [Modifying a variable](#modifying-a-variable)
- [Mutable variables](#mutable-variables)

# Variables📦
## Declaring a variable
To declare a variable, we use the keyword `let` followed by the name of the variable, and the value of the variable.

```rust
let monkeys = 5;
```
We now have a variable `monkeys` with the value `5`.
## Printing a variable💬
We can now use the variable `monkeys` in our program.
For example, we can print the value of `monkeys`:

```rust
let x = 5;
println!("There are {} Monkeys 🐒", monkeys);
```
The `{}` is a placeholder for the value of `x`. It will be replaced by its value when the program is executed.
If we run the program, we will see the following output:
```
There are 5 Monkeys 🐒
```
This program does the same as if we had written:
```rust
println!("There are {} Monkeys 🐒", 5);
```
because `monkeys` is replaced by its value.
## Modifying a variable
We can change the value of a variable by using the following syntax:

```rust
// declaring the variable
let dogs = 5;
// modifying the variable
dogs = 6;
```
But if we run this program, we will get the following error ⛔  :
![](1.png)

We get this error because, by default, variables are immutable. It means that we can't change their value.

## Mutable variables
We can set the variable to be mutable by using the keyword `mut` before the name of the variable.

```rust
let mut dogs = 5;
dogs = 6;
println!("There are {} dogs 🐕", dogs);
```

Output:
```
There are 6 dogs 🐕
```

*And that's how we declare and use variables !*


---

<p align="right"><a href="https://github.com/SkwalExe/learn-rust/tree/main/course/variable-data-types">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>