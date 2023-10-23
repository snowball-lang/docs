# 🤖 Functions

Functions are first-class objects like i32 or char and can be stored in addresses, passed as function parameters or returned by a function. Functions can be defined in many ways and can fill different purposes.\
\
Functions are called by value. This means that `f(1)` calls the function which is the value of the variable `f`. If the value does not have a function type, it will raise a compiler error.

```nim
func myFunc() {
    // Some semi-readable code here :)
}
```

{% content-ref url="basic-syntax.md" %}
[basic-syntax.md](basic-syntax.md)
{% endcontent-ref %}
