---
layout: default
title: 标签 Tags
---

# 标签 Tags

{% assign tags = site.tags | sort %}
{% for tag in tags %}
- <a href="#{{ tag[0] }}">{{ tag[0] }}</a>（{{ tag[1].size }} 篇）
{% endfor %}

<hr>

{% for tag in tags %}
## {{ tag[0] }}
{% for post in tag[1] %}
- <a href="{{ post.url }}">{{ post.title }}</a> <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}
{% endfor %}