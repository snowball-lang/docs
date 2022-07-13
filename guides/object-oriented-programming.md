# Object Oriented Programming

## What is a class?

A class in snowball is a user-defined type or data structure declared with keyword class that has data and functions as its members whose access is governed by the three access specifiers private or public.

By default, these access specifiers are considerated as private. You can change the access specifier by adding the keywords `priv` or `pub`

Snowball classes can also have static properties/methods. You can define one by adding the `static` keyword before a function.

## Public / Private

## Static functions/Attributes

As mentioned before, static functions are defined by adding the `static` keyword before a function declaration. Node that the static keyword should be after pub/priv keyword or else it will result in a syntax error.

{% code title="main.sn" %}
```rust
class MyClass {
    ...
    
    pub static var foo = "bar";
    priv static var foo = "bar";
    static var foo = "bar";
    
    pub static fn my_static_fn() {}
    priv static fn my_static_fn() {}
    static fn my_static_fn() {}
}
```
{% endcode %}

To call a static method or access an attribute, you don't need a new instance of a class, you can just directly accessing by using the `::`symbol. E.g. `MyClass::static_fn()`

{% hint style="info" %}
The `self` variable will not be set if the function is static.

```
class MyClass {
    static fn my_static_fn() {
        self.foo()
        // VariableError: Self is not defined
    }
}
```
{% endhint %}
