# 🔀 Reference types

In Snowball, reference types allow you to create safe references to other values or objects without exposing low-level pointer manipulation. These references provide a way to access and work with data stored elsewhere in memory. Here's the syntax for reference types in Snowball:

```rust
T&
```

In Snowball, these reference types provide a higher level of abstraction compared to raw pointers, ensuring memory safety and preventing common programming errors like null pointer dereferences and dangling pointers. The references automatically handle memory management, making it easier to work with data while minimizing the risk of memory-related bugs.

```rust
fn example(x: myStruct&) {
    a.field = 54;
}

let a: myStruct = ...; // a.field = 10
example(a)             // a.field = 54
```

By using reference types, you can create references to existing values and safely interact with them without directly manipulating memory addresses. Snowball's reference types enable you to write code that is easier to reason about, maintain, and debug.

{% hint style="info" %}
**Reference to a reference, to a reference to a...**

You can create as many references as you want (but it's not recomended). for example:

```rust
let a: i32&&&&...
```
{% endhint %}
