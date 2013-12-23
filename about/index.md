---
title: About
layout: page
comments: no
---

{{ site.about }}

----

###Contact

{% if site.qq %}
QQ : [{{ site.qq }}](tencent://message/?uin={{ site.qq }})
{% endif %}
SITE : [{{ site.name }}]({{ site.url }})

MAIL : [{{ site.email }}](mailto:{{ site.email }})

GitHub : [http://github.com/{{ site.github }}](http://github.com/{{ site.github }})

----

<!--[![weibo](http://service.t.sina.com.cn/widget/qmd/{{ site.weibo }}/223d74f3/1.png)](http://weibo.com/u/{{ site.weibo }})--!>
[![weibo](http://service.t.sina.com.cn/widget/qmd/1406911183/223d74f3/1.png)](http://weibo.com/wz125)
