# 😴 Generics

### How to declare generic parameters

Gneric parameters have the same syntax for classes/struct/interfaces and functions.

```kotlin
class MyOwnInsanelyFastList<T> {...}
```

```rust
fn important_function<T>() {...}
```

The overall syntax is&#x20;

```
[name]<[...[<generic name>: [where clause] [ = <default type>]]]>
```

{% hint style="info" %}
Neither classes/functions/etc... are typechecked if they contain generics

**note:** `fn hello<>() {...}` counts as a generic function
{% endhint %}

### Where clause

The `where clause` is used as a way to make sure the correct generic has been passed.

TODO
