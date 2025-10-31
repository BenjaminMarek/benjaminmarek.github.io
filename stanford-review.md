---
layout: default
title: "Stanford Review Articles"
permalink: /review/
---

# Stanford Review Articles

*The Stanford Review* is Stanford's independent student newspaper, focused on fostering alternative viewpoints and rational debate.

[My *Stanford Review* Profile](https://stanfordreview.org/author/ben-marek/)

## My Review Articles on This Site

{% for post in site.posts %}
{% if post.categories contains "review" %}
- [{{ post.title }}]({{ post.url }}) <small>({{ post.date | date: "%B %Y" }})</small>
{% endif %}
{% endfor %}
