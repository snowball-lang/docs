# System

The System module can be imported from `System`. It offers a variety of useful functions for your program.

### print(Any): Void

This function will take anything as a parameter and print its string content to stdout. The string content will be taken from the `__str` method. Read more about magic methods in the link below (especially about `__str`).

{% content-ref url="../extras/magic-methods.md" %}
[magic-methods.md](../extras/magic-methods.md)
{% endcontent-ref %}

### input(Optional\<String>): String

The input method gets user input from stdin and returns it as a string.

### println(Any): Void

println essentialy is what the `print` function does, except it also adds a new line.

### exit(Number = 0): Void

There are times where it could be useful to return an error code back to your shell. One example:

```rust
import System

pub fn main() {
    System.exit(4);
    // bash: echo $
    // output: 4
}
```
