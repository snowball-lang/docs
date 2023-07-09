# 🔧 Function Attributes

In Snowball, you can use function attributes to modify the behavior and properties of functions. These attributes provide additional information or instructions to the compiler. Here are a few commonly used function attributes:

1. `[[llvm_function]]`: This attribute allows you to embed LLVM code directly within a function, as mentioned earlier. It enables low-level optimizations or specific functionality using the LLVM intermediate representation (IR).
2. `[[internal_linkage]]`: This attribute specifies that a function has internal linkage, meaning it is only accessible within the current module or translation unit. Functions with internal linkage cannot be called from other modules.
3. `[[inline]]`: This attribute suggests to the compiler that the function should be inlined, meaning the function body is directly inserted at the call site instead of making a function call. Inlining can potentially improve performance by reducing function call overhead.
4. `[[test]]`: This attribute is often used to mark functions as test cases or test functions. Test functions are typically used for unit testing purposes to verify the correctness of specific code snippets or components.

{% hint style="info" %}
Note that there are still many more to come!
{% endhint %}

Here's an example that demonstrates the usage of these function attributes:

```rust
fn [[llvm_function]] example() {
    // LLVM code here
}

fn [[internal_linkage]] fn internalFunction() {
    // Function body
}

fn [[inline]] fn inlineFunction() {
    // Function body
}

fn [[test]] fn testFunction() {
    // Function body for testing
    // note: It will be not generate if it's not compiled
    //       with "--test" mode
}
```

In this example, the `example` function uses the `[[llvm_function]]` attribute to embed LLVM code. The `internalFunction` is marked with `[[internal_linkage]]`, indicating that it has internal linkage. The `inlineFunction` is annotated with `[[inline]]`, suggesting the compiler to inline the function when appropriate. Finally, the `testFunction` is marked with `[[test]]`, indicating that it serves as a test function.

By using function attributes, you can customize the behavior and optimize the performance of your Snowball functions, as well as provide additional information for testing or other purposes.

{% content-ref url="../../snowball-cli-usage/testing-mode.md" %}
[testing-mode.md](../../snowball-cli-usage/testing-mode.md)
{% endcontent-ref %}

{% content-ref url="llvm-functions.md" %}
[llvm-functions.md](llvm-functions.md)
{% endcontent-ref %}
