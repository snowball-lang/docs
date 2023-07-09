# 🔄 Casting

In Snowball, casting refers to the process of converting a value from one type to another. It allows you to explicitly change the interpretation or representation of data to match a different type. Casting is useful when you need to perform operations that require compatible types or when you want to ensure proper type compatibility. Here are the casting mechanisms available in Snowball:

```rust
let a = myInteger as f32; // 'a' has a type of f32 now
```

This type of casting is used to explicitly convert a value to a specified target type. The target type must be compatible with the original value, ensuring proper type conversion. Casting to parent types is allowed, while casting to child types requires the use of `dyn_cast<...>(...)` to perform dynamic type checking.

