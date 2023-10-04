# ✨ Builtin macros

### @`pkg`(e: `expr`)

When macros are called, they mutate the context from where they are called. By using the `@pkg` macro, the expression given in is executed INSIDE where the macro has been declared.

```rust
// two.sn
class Hello {}

macro example1() = new Hello();  
macro example2() = @pkg(new Hello());

// one.sn

class Hello {}

...

@example1() // Calls one::Hello
@example2() // Calls two::Hello
```
