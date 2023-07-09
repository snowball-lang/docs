# 🔓 Mutability

In Snowball, you can specify the mutability of variables and data to control whether they can be modified or remain immutable. Mutability is an important aspect of programming languages as it determines the ability to change values.

```rust
T     // unmutable by default
mut T // mutable type for 'T'
```

By distinguishing between immutable and mutable values, Snowball ensures that data is handled appropriately based on the intended use and requirements. Immutable values promote safety and prevent accidental modifications, while mutable values provide flexibility and allow for updates when necessary.

{% hint style="warning" %}
It's important to use mutability judiciously and avoid unnecessary mutations. Immutable values are preferred when possible as they simplify program understanding and reasoning, reduce the chance of bugs, and facilitate code optimizations.
{% endhint %}

{% content-ref url="../casting/mutability-casting.md" %}
[mutability-casting.md](../casting/mutability-casting.md)
{% endcontent-ref %}
