# 🔖 Type aliases

In Snowball, type aliases allow you to create alternative names for existing types, providing convenience and improving code readability. They serve as shorthand for complex or lengthy type definitions, making your code more expressive and understandable. Here's how type aliases are defined in Snowball:

For example, consider the following type alias:

```rust
type PersonID = i32;
```

In this case, `PersonID` is a type alias for the existing `i32` type. You can now use `PersonID` instead of `i32` throughout your code, providing a more meaningful and self-descriptive name when dealing with person identifiers.

Type aliases help in reducing repetition and improving code maintainability. They can be particularly useful when working with complex data structures, function signatures, or custom types. By providing clear and concise names for types, type aliases enhance code comprehension and make it easier to identify the purpose and usage of specific data.

Using type aliases allows you to give semantic meaning to your types, aiding in code documentation and making the intent of your code more evident to others who read it.
