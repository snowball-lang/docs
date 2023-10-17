# 😵 Function Generics

Function templates are special functions that can operate with _generic types_. This allows us to create a function template whose functionality can be adapted to more than one type or class without repeating the entire code for each type.

A template parameter is a special kind of parameter that can be used to pass a type as argument: just like regular function parameters can be used to pass values to a function, template parameters allow to pass also types to a function. These function templates can use these parameters as if they were any other regular type.

{% hint style="info" %}
**Not typechecked!**\
\
Generic functions aren't typechecked until called or used.

<pre class="language-rust"><code class="lang-rust"><a data-footnote-ref href="#user-content-fn-1">fn hello&#x3C;>() {...}</a>
</code></pre>
{% endhint %}



[^1]: This is considered as a generic function!
