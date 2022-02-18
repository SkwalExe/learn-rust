# Learn Rust 🦀 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?url=https%3A%2F%2Fgithub.com%2FSkwalExe%2Flearn-rust&text=Started%20learning%20rust%20with%20@SkwalExe%20learn-rust%20project)

![banner](images/banner.png)

This course was inspired by [Dcode](https://www.youtube.com/watch?v=vOMJlQ5B-M0&list=PLVvjrrRCBy2JSHf9tGxGKJ-bYAN_uDCUL)

Before starting to learn a programming language, you need to understand the basics of programming, **the algorithmics**. 🤓

**Are you french ? This course is available in french [here](https://github.com/SkwalExe/apprendre-rust/)**

# Table of Contents 📚
1. [Installing Rust 🦀](https://github.com/SkwalExe/learn-rust/tree/main/course/installing-rust/)
    - [Linux 😎](https://github.com/SkwalExe/learn-rust/tree/main/course/installing-rust#linux)
    - [Windows 💩](https://github.com/SkwalExe/learn-rust/tree/main/course/installing-rust#windows)
1. [Hello World 👋](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world/)
    - [Declaring a function](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world/#declaring-a-function)
    - [Printing a message 💬](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world/#printing-a-message)
    - [Compiling and running a program🏃‍](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world/#compiling-and-running-a-program) 

1. [Hello World with cargo 🚢](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world-cargo/)
    - [What is cargo❓](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world-cargo#what-is-cargo)
    - [Creating a new project🆕](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world-cargo#creating-a-new-project)
    - [Compiling and running a program with cargo🏃‍](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world-cargo#compiling-and-running-a-program-with-cargo)
        - [Just compiling](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world-cargo#just-compiling)
        - [Compiling and running🏃‍](https://github.com/SkwalExe/learn-rust/tree/main/course/hello-world-cargo#compiling-and-running)

1. [Variables 📦](https://github.com/SkwalExe/learn-rust/tree/main/course/variables/)
    - [Declaring a variable](https://github.com/SkwalExe/learn-rust/tree/main/course/variables#declaring-a-variable)
    - [Printing a variable💬](https://github.com/SkwalExe/learn-rust/tree/main/course/variables#printing-a-variable)
    - [Modifying a variable](https://github.com/SkwalExe/learn-rust/tree/main/course/variables#modifying-a-variable)
    - [Mutable variables](https://github.com/SkwalExe/learn-rust/tree/main/course/variables#mutable-variables)

1. [Variable data types](https://github.com/SkwalExe/learn-rust/tree/main/course/variable-data-types/)
    - [What are data types❓](https://github.com/SkwalExe/learn-rust/tree/main/course/variable-data-types#what-are-data-types)
    - [Specifying data types](https://github.com/SkwalExe/learn-rust/tree/main/course/variable-data-types#specifying-data-types)

1. [if else statements ❓](https://github.com/SkwalExe/learn-rust/tree/main/course/if-else-statements/)
    - [comparison operators](https://github.com/SkwalExe/learn-rust/tree/main/course/variable-data-types#comparison-operators)
    - [if](https://github.com/SkwalExe/learn-rust/tree/main/course/variable-data-types#if)
    - [else](https://github.com/SkwalExe/learn-rust/tree/main/course/variable-data-types#else)
    - [else if](https://github.com/SkwalExe/learn-rust/tree/main/course/variable-data-types#else-if)
1. [Infinite loops ♾️](https://github.com/SkwalExe/learn-rust/tree/main/course/infinite-loops/)
    - [the loop keyword ♾️](https://github.com/SkwalExe/learn-rust/tree/main/course/if-else-statements#the-loop-keyword)
    - [the break keyword 🛑](https://github.com/SkwalExe/learn-rust/tree/main/course/if-else-statements#the-break-keyword)
    - [the continue keyword ➡️](https://github.com/SkwalExe/learn-rust/tree/main/course/if-else-statements#the-continue-keyword)

1. [While loops 🔁](https://github.com/SkwalExe/learn-rust/tree/main/course/while-loops/)
    - [What is a while loop ❓](https://github.com/SkwalExe/learn-rust/tree/main/course/while-loops#what-is-a-while-loop)
    - [The while keyword 🔁](https://github.com/SkwalExe/learn-rust/tree/main/course/while-loops#the-while-keyword)
    - [The break and continue keywords 🔑](https://github.com/SkwalExe/learn-rust/tree/main/course/while-loops#the-break-and-continue-keywords)

1. [For loops 🔢](https://github.com/SkwalExe/learn-rust/tree/main/course/for-loops/)
    - [What is a for loop ❓](https://github.com/SkwalExe/learn-rust/tree/main/course/for-loops#what-is-a-for-loop)
    - [The `for` keyword 🔑](https://github.com/SkwalExe/learn-rust/tree/main/course/for-loopsthe-for-keyword)
    - [Vector iteration](https://github.com/SkwalExe/learn-rust/tree/main/course/for-loops#vector-iteration)
        - [What is a vector❓](https://github.com/SkwalExe/learn-rust/tree/main/course/for-loops#what-is-a-vector)
        - [Declaring a vector](https://github.com/SkwalExe/learn-rust/tree/main/course/for-loops#declaring-a-vector)
        - [Iterating over a vector](https://github.com/SkwalExe/learn-rust/tree/main/course/for-loops#iterating-over-a-vector)
        - [Iterating over a vector with index 🔢](https://github.com/SkwalExe/learn-rust/tree/main/course/for-loops#iterating-over-a-vector-with-index)


# Have a question, want to show your project ?
### **You can open the Discussion 💬 tab on the top right corner of this page.**
![discussion](images/discussions.png)
# final
If you have any probleme, don't hesitate to open an issue
# contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
## Todo
- [ ] Add a section about the Rust language
- [ ] Add installation instructions for macOS