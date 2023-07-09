# 🔐 Mutability casting

In Snowball, mutability casts provide a way to change the mutability of a variable or reference. It allows you to convert a mutable value into an immutable value, providing flexibility in managing the mutability of data. Here's how mutability casts are performed in Snowball:

<pre class="language-rust"><code class="lang-rust"><strong>let mut a: i32 = ...; // "a" is mutable
</strong><strong>x(a as i32);     // "b" is no longer mutable 
</strong></code></pre>

By using mutability casts, you can adapt the mutability of values or references to suit your specific needs. This allows you to control how data is accessed and modified within your program, promoting safer and more flexible code.
