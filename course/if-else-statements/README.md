# Table of Contentsπ

- [comparison operators](#comparison-operators)
- [if](#if)
- [else](#else)
- [else if](#else-if)

# if else statements 

## comparison operators

The comparison operators are used to compare two values.

| Operator | Description              |
| -------- | ------------------------ |
| ==       | equal to                 |
| !=       | not equal to             |
| >        | greater than             |
| <        | less than                |
| >=       | greater than or equal to |
| <=       | less than or equal to    |

## if

Imagine that you are a programmer and you have to write a program that will tell if the value of a variable is positive

```rust
let x = 5;
```

For that, you will have to check if `x` is superior to 0.

We can do that with the `if` statement.

```rust
if x > 0 {
    println!("x is positive π");
}
```

The code between the `{}` will be executed because the condition `x > 0` is true.

If we change the value of `x` to a negative number, the code between the `{}` will not be executed.

## else 

Imagine that you are a programmer and you have to write a program that will say hello if the value of a variable is equal to 5, and goodbye if it is not.

To do that, you will first have to check if `x` is equal to 5, and then use the else statement to say goodbye if the condition is not true.

```rust
if x == 5 {
    println!("Hello π");
} else {
    println!("Goodbye π«");
}
```

Let's run the code with `x = 5`:

```
Hello π
```

And with `x = 6`:

```
Goodbye π«
```

## else if

It is possible to have more than one condition to be checked.

Imagine that we want to say hello if `x` is equal to 5, good morning if it is equal to 6, and good night if either of the two conditions is not true.

we can do that with the `else if` statement.

```rust
if x == 5 {
    println!("Hello π");
} else if x == 6 {
    println!("Good morning π");
} else {
    println!("Good night π");
}
```

lets run the code with `x = 5`:

```
Hello π
```

And with `x = 6`:

```
Good morning π
```

And with `x = 7`:

```
Good night π
```

> βΉοΈ We can put as many `else if` as we want. The condition of the `else if` will be checked after the condition of the previous `else if`.

---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home π </a> - <a href="../infinite-loops">Next Section β­οΈ</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>