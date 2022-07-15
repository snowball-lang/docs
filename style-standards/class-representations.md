# Class Representations

Class representations are essential for debugging meaning that these "official" representations should contain useful information that the user might need. The first word in the string should be the class's name followed by `()` as if it was a function call. Then, if any variables are needed to be shown, they should contain the name, followed by an equal sign and the value (each variable separated by spaces).

some examples:

* Default representation created by Snowball

```
Foo( located at 0x... )
```

* Representation with variables

```
Foo( bar="hello" snowball=25 )
```
