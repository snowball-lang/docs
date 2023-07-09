# ⁉ Type Generics

In Snowball, type generics enable you to write reusable code that can operate on different types. They allow you to create functions, data structures, and components that can adapt to various data types without sacrificing type safety. Type generics in Snowball are denoted by `<...>` and provide flexibility and versatility in your code. Here's how type generics are used in Snowball:

```rust
let a: Vector<i32>;
```

* In this example we are pointing to a vector type that has the first generic argument as `i32`.

{% hint style="success" %}
Using type generics inside expressions.

Generic types can be defined using **`< ... >`** in places where snowball expects a type. But in other places such as in function arguments, we would need to provide an extra **`?`** symbol to differentiate the expression from being a **`less than operator`**.

```rust
let a = myFunction<?i32>();
```
{% endhint %}
