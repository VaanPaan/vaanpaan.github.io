---
layout: page
title: 正文
order: 2
permalink: /articles/
---

{% assign articles = site.posts | where: "categories", "ITSM" | sort: "date" %}
{% for post in articles %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p style="color: gray;">{{ post.date | date: "%Y-%m-%d" }}</p>
  <p>{{ post.excerpt }}</p>
{% endfor %}
