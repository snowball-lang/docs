# 💢 LLVM Functions

In Snowball, you can embed LLVM code within a function using the `[[llvm_function]]` attribute. This allows you to directly write LLVM code for low-level optimizations or specific functionality. Here's an example of how to define an LLVM function in Snowball:

```swift
@llvm_function
func example() {
    // LLVM code here
}
```

When defining an LLVM function, you have the flexibility to write low-level code directly using the LLVM intermediate representation (IR). Here's a simple example of LLVM code within an LLVM function:

```swift
@llvm_function
func example() {
    %add = add i32 2, 3   ; Add 2 and 3, result stored in %add
    ret i32 %add          ; Return the value stored in %add
}
```

In this example, the LLVM code performs an addition operation between the integers 2 and 3. The result is stored in the `%add` register, and then it is returned using the `ret` instruction.

By using the `llvm_function` attribute, you can leverage the power and flexibility of LLVM to optimize specific sections of your Snowball code or implement functionality that requires fine-grained control over the machine-level operations.

Please note that writing LLVM code requires a good understanding of the LLVM IR and low-level optimizations. Be cautious while using LLVM functions and ensure that they are used appropriately and sparingly within your Snowball programs.

{% hint style="warning" %}
Snowball should provide you with the necessary tools to create virtually anything but this feature exists in case something requires more low-level unsafeness.
{% endhint %}
