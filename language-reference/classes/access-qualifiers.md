# 🔒 Access qualifiers

In Snowball, access qualifiers determine the visibility and accessibility of class members (variables and methods) from outside the class. Snowball provides three access qualifiers: `pub`, `priv`.&#x20;

These qualifiers allow you to control the level of encapsulation and restrict or expose class members as needed. Here's an explanation of each access qualifier:

```rust
class Foo {
  let a: char& = "hello"; // private scope
  pub:
    let b: i32 = 0; // public scope
  priv:
    let c: f32 = 1.2; // private scope, again
}
```
