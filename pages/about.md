---
layout: page
title: About
description: 有态度的码农
keywords: ChuanZhi, 传智
comments: true
menu: 关于
permalink: /about/
---

我是李传智，做一个有态度的码农。

编程也是一项艺术，努力把每一个作品做到最好。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
