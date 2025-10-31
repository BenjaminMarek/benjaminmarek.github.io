---
layout: default
title: "Stanford Review Articles"
permalink: /review/
---

# Stanford Review Articles

<a href="https://stanfordreview.org/author/ben-marek/">Stanford Review Profile</a>

### My Articles on This Site

{% for post in site.posts %}
{% if post.categories contains "review" %}
- [{{ post.title }}]({{ post.url }}) <small>({{ post.date | date: "%B %Y" }})</small>
{% endif %}
{% endfor %}
