# 🔢 Primitive types

Snowball provides a set of primitive types that serve as the building blocks for representing basic data in your programs. These types are essential for storing and manipulating fundamental values. Here are the primitive types in Snowball:

### Integer types

* `i[n]`: n-bit signed integer type.
  * examples: `i32`, `i64`, `i39`
* `u[n]`: n-bit unsigned integer type.
  * examples: `u8`, `u32`, `u128`

{% hint style="warning" %}
Integer type sizes can only go from **1** (`bool`) to **2^23** (**8,388,608**)
{% endhint %}

### Floating-Point Types

* `f32`: 32-bit floating-point type (single-precision).
* `f64`: 64-bit floating-point type (double-precision).
* `f16`: (Not implemented yet!)

### Boolean Type

* `bool`: A Boolean type representing either `true` or `false`.

### Character Type:

* `char`: A character type representing a single Unicode character. (**u8**)

### Other unsized types

These are types that do not implement the `Sized` trait, and therefor, it can't be used in variables, arguments, etc...

* `void`: the return type of a function that returns normally, but does not provide a result value to its caller. **It can be used as an** [**unknown pointer type**](unknown-pointer-type-void-pointers.md)**!**

{% content-ref url="reference-types.md" %}
[reference-types.md](reference-types.md)
{% endcontent-ref %}

These primitive types provide the foundation for representing and manipulating various kinds of data in Snowball programs. They have different sizes and properties, allowing you to choose the appropriate type based on your specific requirements.

By understanding and utilizing these primitive types effectively, you can perform arithmetic operations, and logical evaluations, and handle textual data within your Snowball programs.
