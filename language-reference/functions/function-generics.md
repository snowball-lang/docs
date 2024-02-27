# 😵 Function Generics

Function generics are special functions that can operate with _generic types_. This allows us to create a function template whose functionality can be adapted to multiple types or classes without repeating the entire code for each type.

A template parameter is a special parameter that can be used to pass a type as an argument: just like regular function parameters can be used to pass values to a function, template parameters allow to pass also types to a function. These function templates can use these parameters like any other regular type.

```swift
func add<T>(a: T, b: T) {
    return a + b;
}

add(1,2) // 3
add("hello-", "world") // hello-world
```

### Generics 101

{% content-ref url="../generics.md" %}
[generics.md](../generics.md)
{% endcontent-ref %}

