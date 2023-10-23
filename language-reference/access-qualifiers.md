# 🔏 Access qualifiers

Snowball provides access qualifiers that allow you to control the visibility and accessibility of various program elements within modules, namespaces, and classes. These qualifiers ensure proper encapsulation and information hiding, promoting code organization and maintainability. Let's explore access qualifiers in different contexts:

```swift
namespace x {
 func test() {
    // ...
 }
}
...
x::test(); // error: can't access private function from this context
```

Remember to carefully consider the desired level of visibility for each program element and choose the appropriate access qualifier accordingly.

{% hint style="success" %}
```swift
namespace x {
 public func test() {
    // ...
 }
}
```
{% endhint %}
