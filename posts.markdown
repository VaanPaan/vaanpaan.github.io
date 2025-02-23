---
layout: page
title: 所有文章
order: 2
permalink: /articles/
---

# 所有文章

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
{% endfor %}
