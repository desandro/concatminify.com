---
layout: page
---

# Concat & minify

Concatenating and minifying your JavaScript and CSS files is an easy way to make websites faster.

## Concatenation 

For every CSS, JS, and image file used in a page's HTML, devices have to make a separate HTTP request to get it.

{% highlight html %}
<!-- CSS -->
<link rel="stylesheet" href="/css/base.css" /> <!-- request -->
<link rel="stylesheet" href="/css/layout.css" /> <!-- request -->
<link rel="stylesheet" href="/css/modules.css" /> <!-- request -->
<!-- JS -->
<script src="/js/plugin-a.js"></script> <!-- request -->
<script src="/js/plugin-b.js"></script> <!-- request -->
<script src="/js/page.js"></script> <!-- request -->
{% endhighlight %}

Concatenation merges several files into one, so devices make fewer requests. Reducing the number of these HTTP requests makes websites faster.

{% highlight html %}
<!-- CSS, concat all .css files in styles.css -->
<link rel="stylesheet" href="/css/styles.css"> <!-- request -->
<!-- JS, concat all .js files in scripts.js -->
<script src="/js/scripts.js"></script> <!-- request -->
{% endhighlight %}

## Minification

