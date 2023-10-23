# 😴 Generics

### How to declare generic parameters

Generic parameters have the same syntax for classes/struct/interfaces and functions.

```kotlin
class MyOwnInsanelyFastList<T> {...}
```

```swift
func important_function<T>() {...}
```

The overall syntax is&#x20;

```
[name]<[...[<generic name>: [where clause] [ = <default type>]]]>
```

{% hint style="info" %}
Neither classes/functions/etc... are type-checked if they contain generics

**note:** `fn hello<>() {...}` counts as a generic function
{% endhint %}

### Where clause

The `where clause` is used as a way to make sure the correct generic has been passed. For example, let's imagine you are making a vector class that only what's `T` to be a `Sized` type. (all types implement Sized except those whose size is not known at compile time, for example, `void`)

```typescript
class MyVector<T: Sized> {...}
```

Here, snowball checks if the given generics `implements` the given types.

```typescript
let a: MyVector<void> // error: void doesn't implement "Sized"
let b: MyVector<i32> // ok
```

{% hint style="info" %}
You can declare `where` clauses separately to either check for other types or better reading:

```swift
class Vector<T: Sized> {
   func to_string<>() 
      where T: ToString
   { ... } 
}
```
{% endhint %}
