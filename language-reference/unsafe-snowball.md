# 🔫 Unsafe snowball

"Unsafe Snowball" refers to a variant or mode of the Snowball programming language that allows for more low-level operations and memory access, similar to "unsafe" features in other programming languages like C or C++. In Snowball, "unsafe" code typically bypasses some of the safety checks enforced by the language's standard mode, allowing for more direct control over memory and system resources.



### Dereference of a raw pointer

```rust
let mut num = 5;
let r1 = &num as *const i32;

unsafe {
    let x = *r1; // only in unsafe blocks!
}
```

### Calling unsafe functions

Snowball typically refer to specific function or method invocations that are marked as "unsafe." These calls are used when a developer needs to perform operations that can potentially lead to undefined behavior, memory safety issues, or other risks. In Snowball, the "unsafe" keyword is often used to indicate such calls.

```rust
unsafe func dangerous() { ... }
    
unsafe {
    dangerous(); // ok, if you are cool with it ¯\_(ツ)_/¯
}

dangerous(); // nah, you can't do that here!
```

### Pointer arithmetic

Unsafe Snowball might allow direct pointer arithmetic, enabling manipulation of memory addresses. This can be error-prone and risky if not used carefully.

**TODO TODO TODO TODO TODO**
