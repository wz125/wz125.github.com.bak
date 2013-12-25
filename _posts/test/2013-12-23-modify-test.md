---
layout: post
title: 'modiy-test'
category: 'test'
tags: [syntax]
---

Modify
--

+ Latex()
    1. add javascript
{% highlight javascript linenos %}
    <!-- MathJax Section -->
    <script type="text/javascript"
    src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
    <script>
    MathJax.Hub.Config({
          tex2jax: {
          skipTags: ['script', 'noscript', 'style', 'textarea', 'pre']
          }
    });
    MathJax.Hub.Queue(function() {
        var all = MathJax.Hub.getAllJax(), i;
        for(i=0; i < all.length; i += 1) {
            all[i].SourceElement().parentNode.className += ' has-jax';
        }
    });
    </script>
{% endhighlight %}
<!----!>
    2. add css
{% highlight css linenos %}
body div.content {}
    body div.content code.has-jax {
            font: inherit;
            font-size: 100%;
            background: inherit;
            border: inherit;
            color: #000000;
        }
{% endhighlight %}

+ Syntax()
+ duoshuo()
+ Outliner(outliner.js )
+ weibo pic sign
+ /categories/categories.html(test)

Thanks
--

+ clone [yonsm.net](https://github.com/Yonsm/NET)
+ refer [mad4a.me](http://github.com/89ao)
+ refer [zhangjunhd.github.io](https://github.com/zhangjunhd)


