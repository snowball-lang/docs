# 💅 The desired standard

A "perfect" coding style for an object-oriented programming language like Snowball is subjective, and it can vary depending on your team's preferences and project requirements. However, this is the official standard Snowball uses for their projects and is considered the best practice.

## Naming Conventions

It's recommended to use lowercase letters for variable names, with words separated by underscores (snake\_case).&#x20;

```rust
let length = 25;
let mut my_class;
```

Class names should use CamelCase, with the first letter of each word capitalized. They shall be descriptive and full worded too!

```kotlin
// Good!
class MyClass {}

// Meh...
class MyVectorIter {} // suggestion: MyVectorIterator

// Absolutely not! 🤮
// * Start's with lowercase
// * No clear word case
class _Hello_there {}
```

Function names should also use lowercase letters with words separated by underscores.&#x20;

```nim
👍 func print_something() {}
👎 func PrintSomething() {}
```

Additionally, it's important to choose descriptive names that accurately and succinctly reflect the purpose and function of the variable, class, or function.

## Class syntax

In the snowball source code, we use tabs with 2 spaces only. This makes it good to create a clear and concise syntax declaration for the class.

Static functions should be bottom of the class and private/public in separate blocks.

```kotlin
class Application {
    let title: String = "";
  public:
    Application() {}
    func get_title() { ... }
}
```

