---
layout: post-light-feature
title: 尾递归的迭代形式化
description: "尾递归"
category: articles
tags: [Programming, FP]
---

~~~ ocaml
let rec fact n = if n = 0 then 1 else n*(fact (n-1));;
~~~

$$
a^2+b^2=c^2
$$


$$
a^2+b^2=c^2 \\
a^2+b^2=c^2 \\
\sum_{i=0}^n a_i
$$

For example fenced code

~~~ ruby
print "Hello World"
~~~

~~~ ocaml
let fact = let rec f ans n = 
		if n = 0 then ans 
		else f (ans*n) (n-1) 
~~~

~~~ ocaml
let fact = let rec f ans n = 
		if n = 0 then ans 
		else f (ans*n) (n-1) 
	in f 1;;
~~~

{% highlight c %}
#include <stdio.h>

int main()
{
	return 0;
}
{% endhighlight %}


{% highlight html linenos %}
<figure>
    <img src="/images/image-filename-1.jpg">
    <figcaption>Caption describing these two images.</figcaption>
</figure>
{% endhighlight %}