# 💼 Members

In Snowball, class variables are members of a class that are shared among all instances of the class. They are also known as static variables or class-level variables. Class variables maintain their value across different instances of the class and can be accessed directly through the class itself. Here's an explanation of class variables in Snowball:

You **must** specify the variable type when declaring a class member.

```rust
class Y {
    let x: i32;
           ^^^
}
```

{% hint style="info" %}
Variables can have default initializers and they will be initialized when the constructor is called.
{% endhint %}
