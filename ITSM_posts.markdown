---
layout: page
title: IT管理
order: 2
permalink: /ITSM/
---

{% assign itsm_posts = site.posts | where: "categories", "ITSM" | sort: "date" %}
{% for post in itsm_posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p style="color: gray;">{{ post.date | date: "%Y-%m-%d" }}</p>
  <p>{{ post.excerpt }}</p>
{% endfor %}
