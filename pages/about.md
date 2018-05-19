---
layout: page
title: About
description: 阿力的博客
keywords: 测试, 测试开发, 爱吐槽, 电影狂
comments: true
menu: 关于
permalink: /about/
---

我是阿力

努力是唯一出路

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
