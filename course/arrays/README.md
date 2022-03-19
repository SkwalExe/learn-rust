# Table of contents📚

- [What is an array❔](#what-is-an-array)
- [Declaring an array](#declaring-an-array)
- [Accessing an array](#accessing-an-array)
- [Iterating over an array🔁](#iterating-over-an-array)
  - [With the iter method](#with-the-iter-method)
  - [With the length of the array](#with-the-length-of-the-array)
- [Specifying the type and the length of an array](#specifying-the-type-and-the-length-of-an-array)
- [Default values for arrays](#default-values-for-arrays)

# Arrays 📜

## What is an array❔

An array is a collection of items of the same type. It is similar to tuples, but tuples can contain different types of items.

## Declaring an array

To declare an array, we use the `[]` brackets, and the different items separated by commas.

```rust
let objetcs_array = ['👓', '👕', '🧽', '🩴', '🧲'];
```

## Accessing an array

To access an item in an array, we use the index of the item.

```rust
println!("I like {} and {}", objects_array[0], objects_array[1]);
```

Output:

```
I like 👓 and 👕
```

## Iterating over an array🔁

### With the iter method

To iterate over an array, we use the `.iter()` method in a for loop.

```rust
for item in objects_array.iter() {
    println!("I bought a {}", item);
}
```

Output:

```
I bought a 👓
I bought a 👕
I bought a 🧽
I bought a 🩴
I bought a 🧲
```

### With the length of the array

To iterate over an array, we can use the `.len()` method to get the length of the array.

```rust
for i in 0..objects_array.len() {
    println!("I bought a {}", objects_array[i]);
}
```

Output:

```
I bought a 👓
I bought a 👕
I bought a 🧽
I bought a 🩴
I bought a 🧲
```

## Specifying the type and the length of an array

We can specify the type and the length of an array when we declare it by adding `:` and the types and the length separated by semicolons `: [type; length]`.

```rust 
let objects_array: [str; 5] = ["👓", "👕", "🧽", "🩴", "🧲"];
```

## Default values for arrays

We can create an array, we can fill a specific range of indexes with a default value.

```rust
let penguins_army = ['🐧'; 20];
```

We just created an array of 20 penguins.

To see what our array looks like, we will have to use a different jocker in the println! statement.

```rust
println!("{:?}", penguins_army);
```

> ℹ️ The `:?` is a jocker that prints the array like we would see it in the code.

Output:

```
['🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧', '🐧']
```

And we can see that we have an army of penguins 🔫🐧.

---

<p align="right"><a href="../struct-methods">Next Section ⏭️</a></p>

---

<p align="right">Course created by <a href="https://github.com/SkwalExe/" target="_blank">SkwalExe</a> and inspired by <a href="https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL" target="_blank">Dcode</a></p>