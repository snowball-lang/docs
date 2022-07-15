# Magic Methods

In snowball, Magic methods are used to bring better functionality to a class. Some of these new functionalities are things like: operation overload, get attributes/set attributes, constructors, destructors and many more.

### \_\_init

The init method is called whenever a new instance of a class has been created. A new instance of a class is created when the programmer uses the `new` keyword. Arguments can be passed through the new statement and these arguments will be passed to \_\_init. You can overload the init method by having different argument types and it does not need to return anything (and returns are not available in this function). If no constructor has been declared, a default one will be set in order to have a new instance.

```rust
class Foo {
    fn __init(arg1) {
        // called
    }
}

fn main() {
    new Foo("this is an argument")
}
```

### \_\_die

This method is called automatically when an object is about to be destroyed. One of these scenarios can be when a class has gone out of scope. The destructor is used to free memory occupied by the objects created by the constructor. A default deconstructor will be set if none has been defined. This method should not return anything and it can't have any arguments.

### \_\_get

TODO

### \_\_set

TODO

### \_\_sum

The `__sum` method is an operator override. It is called when using the `+` operator. This function can be overloaded by using different argument types. Only one argument is passed to the method and that is the object that you are subtracting from.

```rust
class Vector {
    fn __sum(vec2: Vector) -> Vector {
        return new Vector(self.x + vec2.x)
    }
    
    fn __sum(num2: Number) -> Vector {
        return new Vector(self.x + num2)
    }
}

fn main() {
    var a = new Vector() + new Vector();
    var b = new Vector() + 23;
}
```

### \_\_sub

TODO

### \_\_mul

TODO

### \_\_div

TODO

### \_\_isum

TODO

### \_\_isub

TODO

### \_\_imul

TODO

### \_\_idiv

TODO

### \_\_str

TODO

### \_\_repr

This magical method is used (normally) for debugging purposes. The `__repr` method should return a string and it can't have any arguments. Please, note that `__str` and `__repr` are 2 different functions and they do not share the same purpose.&#x20;

If possible, refer to the Style Standards to know how to represent a class inside a string.

{% content-ref url="../style-standards/class-representations.md" %}
[class-representations.md](../style-standards/class-representations.md)
{% endcontent-ref %}

### \_\_del

TODO (for deleting items)

### \_\_eqeq

TODO

### \_\_eq

TODO
