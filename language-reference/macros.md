# ⚒ Macro

Macros are powerful code transformation tools that allow you to define and reuse code patterns. They provide a way to generate code automatically and perform compile-time code transformations. In Snowball, macros are defined using the `macro` keyword followed by the macro's name. Let's explore macros in detail with different sections:

#### Macro arguments

In snowball. macros are being `type-checked` to provide a better and more secure macro expansion system. These are the current ones that can be used:

* `cosnt`: A generic constant value. This macro type is generic and accepts every type of constant value.
  * `str`: A string constant value.
  * `num`: A constant number (int or real) value.
  * `chr`: A single constant character value.
* `expr`: Any type of expression such as a function call, a constant expression or a variable.
* `stmt`: Any sort of statements such as if statements, while loops and even function definitions.

#### Expression macro

Macros can be used both as a statement and an expression depending on the context. For example:

```rust
macro myFormat(f: cosnt[str], args: ...expr) = ....
                                             ^
```

#### Statement macro

Macros that can be used in a statement value. for example:

```rust
macro callIf(x: expr, c: stmt) {
    if @x {
        @c("example");
    }
}
```

Macros are a powerful feature in Snowball, allowing you to define reusable code patterns and perform code transformations during compilation. When you call a macro using `@macroName()`, the code within the macro definition is inserted at the call site, providing a convenient way to generate code dynamically.
