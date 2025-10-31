---
layout: default
---

### Recent Essays

{% for post in site.posts %}
  {% unless post.categories contains "review" %}
    - [{{ post.title }}]({{ post.url }}) <small>({{ post.date | date: "%B %Y" }})</small>
  {% endunless %}
{% endfor %}
