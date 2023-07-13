# 🔏 Access qualifiers

Snowball provides access qualifiers that allow you to control the visibility and accessibility of various program elements within modules, namespaces, and classes. These qualifiers ensure proper encapsulation and information hiding, promoting code organization and maintainability. Let's explore access qualifiers in different contexts:

```rust
namespace x {
 fn test() {
    // ...
 }
}
...
x::test(); // error: can't access private function form this context
```

Remember to carefully consider the desired level of visibility for each program element and choose the appropriate access qualifier accordingly.

{% hint style="success" %}
```rust
namespace x {
 pub fn test() {
    // ...
 }
}
```
{% endhint %}
