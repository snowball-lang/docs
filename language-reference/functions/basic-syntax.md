---
description: Function arguments and return types
---

# 🐣 Basic syntax

#### Argument list

In Snowball, you can define function arguments using the following syntax:

```nim
func function_name(argument_name: data_type) {
    // Function body
}
```

For example, let's consider a function called `hello` that takes a single argument `x` of type `i32` (32-bit integer). The syntax for defining such a function with an argument in Snowball would be:

```nim
func hello(x: i32) {
    // Function body
}
```

Within the function body, you can access and use the argument `x` as needed to perform operations or calculations. Remember to provide the appropriate data type when invoking the `hello` function and passing values for the argument.

Using the syntax mentioned above, you can define functions with different arguments in Snowball, allowing for flexible and modular code development.

#### Return types

In Snowball, you can specify the return type of a function using the following syntax:

```nim
func function_name() return_type {
    // Function body
    // Return statement
}
```

Using the syntax mentioned above, you can define functions with different return types in Snowball, allowing you to perform computations and provide results based on your program's requirements.

{% hint style="info" %}
**Voided functions**

To declare a function as `void`, there's no need to declare `void` type, just can not put anything:

```nim
func no_returns(a: i32, b: f32) {
    // tada!
}
```
{% endhint %}

{% content-ref url="../types.md" %}
[types.md](../types.md)
{% endcontent-ref %}
