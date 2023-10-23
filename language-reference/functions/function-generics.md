# 😵 Function Generics

Function templates are special functions that can operate with _generic types_. This allows us to create a function template whose functionality can be adapted to multiple types or classes without repeating the entire code for each type.

A template parameter is a special parameter that can be used to pass a type as an argument: just like regular function parameters can be used to pass values to a function, template parameters allow to pass also types to a function. These function templates can use these parameters like any other regular type.

{% hint style="info" %}
**Not type-checked!**\
\
Generic functions aren't typechecked until called or used.

<pre class="language-nim"><code class="lang-nim"><a data-footnote-ref href="#user-content-fn-1">func hello&#x3C;>() {...}</a>
</code></pre>
{% endhint %}

### Generics 101

{% content-ref url="../generics.md" %}
[generics.md](../generics.md)
{% endcontent-ref %}

[^1]: This is considered as a generic function!
