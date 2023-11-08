# 🔧 Function Attributes

In Snowball, you can use function attributes to modify the behaviour and properties of functions. These attributes provide additional information or instructions to the compiler. Here are a few commonly used function attributes:

1. `llvm_function`: As mentioned earlier, This attribute allows you to embed LLVM code directly within a function. It enables low-level optimizations or specific functionality using the LLVM intermediate representation (IR).
   1. `llvm_function(sanitise_void_return)`: This replaces all `void` types in return types and argument types to an `i8` in the llvm IR.
2. `internal_linkage`: This attribute specifies that a function has internal linkage, meaning it is only accessible within the current module or translation unit. Functions with internal linkage cannot be called from other modules.
3. `inline`: This attribute suggests to the compiler that the function should be inlined, meaning the function body is directly inserted at the call site instead of making a function call. Inlining can potentially improve performance by reducing function call overhead.
4. `no_inline`: This tells the compiler to not inline the function.
   1. > `inline` and `no_inline` can't be used in the same function!
5. `test`: This attribute often marks functions as test cases or test functions. Test functions are typically used for unit testing purposes to verify the correctness of specific code snippets or components.
   1. `test(skip=0)`: If it's 1, it will skip the test and it won't be executed.
   2. `test(expect=1)`: It will be the default check value. Default is 1
   3. `test(description = "")`: Add a description to the unit test.
6. `bench`: This attribute marks a function as a benchmarking function. These functions are executed and benchmarked when running `snowball bench`.
7. `no_mangle`: It doesn't mangle the function's name at the executable.
   1. This doesn't work on class functions!
8. `export`: It exports a function with the specified arguments
   1. `export(name="<name>")`: It exports the function as the specified name. Default is the function mangled name.
9. `unsafe_fn_not_body`: This attribute leaves the function marked as `unsafe` but it does not enter in an unsafe context for its block.&#x20;
   1. > They can only be used in `unsafe` functions

{% hint style="info" %}
Note that there are still many more to come!
{% endhint %}

Here's an example that demonstrates the usage of these function attributes:

```swift
@llvm_function
func example() {
    // LLVM code here
}

@internal_linkage
func internalFunction() {
    // Function body
}

@inline
func inlineFunction() {
    // Function body
}

@test(expect = 62)
func testFunction() {
    // Function body for testing
    // note: It will be not generated if it's not compiled
    //       with "--test" mode
}
```

In this example, the `example` function uses the `llvm_function` attribute to embed LLVM code. The `internalFunction` is marked with `internal_linkage`, indicating that it has internal linkage. The `inlineFunction` is annotated with `inline`, suggesting the compiler to inline the function when appropriate. Finally, the `testFunction` is marked with `test`, indicating that it serves as a test function that expects `62`.

By using function attributes, you can customize the behaviour and optimize the performance of your Snowball functions, as well as provide additional information for testing or other purposes.

{% content-ref url="../../snowball-cli-usage/testing-mode.md" %}
[testing-mode.md](../../snowball-cli-usage/testing-mode.md)
{% endcontent-ref %}

{% content-ref url="llvm-functions.md" %}
[llvm-functions.md](llvm-functions.md)
{% endcontent-ref %}
