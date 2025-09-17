
---
layout: default
title: 分类 Categories
---

# 分类 Categories

{% for category in site.categories %}
- <a href="#{{ category[0] }}">{{ category[0] }}</a>（{{ category[1].size }} 篇）
{% endfor %}

<hr>

{% for category in site.categories %}
## {{ category[0] }}
{% for post in category[1] %}
- <a href="{{ post.url }}">{{ post.title }}</a> <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}
{% endfor %}

