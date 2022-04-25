# Defining traits

We will create a trait called `GetType` that we will use to get the type of a variable as a string.

To define a trait we use the `trait` keyword and the name of the trait, followed by the prototype of the methods we want to implement.

```rust
trait GetType {
    fn get_type(&self) -> &str;
}
```

We will implement the `get_type` trait for the `String` type.

```rust
impl GetType for String {
    fn get_type(&self) -> &str {
        "String"
    }
}
```

Now every time the `get_type` method will be called on a `String` instance, it will return the "String".

```rust
let my_string = String::from("Hello world!");

println!("Hi, my name is my_string ! I'm a {} and my value is {}", my_string.get_type(), my_string);
```

Result:

```
Hi, my name is my_string ! I'm a String and my value is Hello world!
```

<!--
---

<p align="right"><a href="https://skwalexe.github.io/learn-rust/">Home 🏠</a> - <a href="../defining-traits">Next Section ⏭️</a></p>
-->

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>