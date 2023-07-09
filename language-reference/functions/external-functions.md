# ❓ External functions

In Snowball, you can declare and use external functions that are implemented outside of your current module or translation unit. This allows you to interface with code written in other programming languages or external libraries. Here are a couple of examples of declaring and using external functions in Snowball:

1. Basic External Function Declaration:

```rust
extern fn example();
```

In this example, `example` is declared as an external function. You can use this declaration to call the function without providing the implementation within your Snowball code. The implementation of `example` is expected to be provided by an external source, such as another module or library.

2. External Function Declaration with Custom Name:

```rust
extern "my.weird$function" as myNormalFn();
```

In this example, `myNormalFn` is declared as an external function with a custom name `"my.weird$function"`. This allows you to specify a specific name for the external function that might differ from its original name or naming conventions. You can then use `myNormalFn` to call the function in your Snowball code.

When declaring external functions, it's important to ensure that the function name and signature match the actual implementation in the external code. This includes the function name, the number and types of arguments, and the return type.

External functions enable Snowball to interact with external code seamlessly, extending the capabilities of your programs by leveraging existing libraries or external functionality.

{% hint style="info" %}
You don't need to specify argument names in external functions, for example:

```rust
extern fn foo(i32, char*, String);
```
{% endhint %}



