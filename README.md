# 😼 Welcome to Snowball

First of all, what is snowball?

* Snowball is a low-weight, statically typed, object oriented programming language with garbage collector and module system.

What are some of it's advantages?

* TODO

Here is a little demonstration to show you how snowball feels like

{% code title="main.sn" %}
```rust
import System

class Vector {

    priv Number x;
    priv Number y;

    pub fn __init(x: Number, y: Number) {
        self.x, self.y = x, y;        
    }
    
    // JS equivalent: const __sum = (this, vec2) => new Vector(...)
    // overrides operator +
    pub fn __sum(vec2: Vector) -> Vector = 
        new Vector(self.x + vec2.x, self.y + vec2.y)
    
    pub fn __str() -> String {
        return "Vector(x=${self.x} y=${self.y})"
    } 
}

fn main(args: Array<String>) -> Number {
    let vec1 = new Vector(1,2)
    let vec2 = new Vector(10,22)
    
    System.print(vec1 + vec2)
    return 0
}
```
{% endcode %}

### Guides: Jump right in

Follow our handy guides to get started on the basics as quickly as possible:

{% content-ref url="guides/object-oriented-programming.md" %}
[object-oriented-programming.md](guides/object-oriented-programming.md)
{% endcontent-ref %}

{% content-ref url="guides/basic-concepts.md" %}
[basic-concepts.md](guides/basic-concepts.md)
{% endcontent-ref %}

{% content-ref url="guides/advanced-concepts.md" %}
[advanced-concepts.md](guides/advanced-concepts.md)
{% endcontent-ref %}

{% hint style="info" %}
**Good to know:** your product docs aren't just a reference of all your features! use them to encourage folks to perform certain actions and discover the value in your product.
{% endhint %}

### Fundamentals: Dive a little deeper

Learn the fundamentals of MyProduct to get a deeper understanding of our main features:

{% content-ref url="fundamentals/projects.md" %}
[projects.md](fundamentals/projects.md)
{% endcontent-ref %}

{% content-ref url="fundamentals/members.md" %}
[members.md](fundamentals/members.md)
{% endcontent-ref %}

{% content-ref url="fundamentals/task-lists.md" %}
[task-lists.md](fundamentals/task-lists.md)
{% endcontent-ref %}

{% content-ref url="fundamentals/tasks.md" %}
[tasks.md](fundamentals/tasks.md)
{% endcontent-ref %}

{% hint style="info" %}
**Good to know:** Splitting your product into fundamental concepts, objects, or areas can be a great way to let readers deep dive into the concepts that matter most to them. Combine guides with this approach to 'fundamentals' and you're well on your way to great documentation!
{% endhint %}
