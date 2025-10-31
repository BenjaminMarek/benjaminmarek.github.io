---
layout: default
---

### Recent Essays

{% for post in site.posts %}
{% if post.categories != review %}
- [{{ post.title }}]({{ post.url }}) <small>({{ post.date | date: "%B %Y" }})</small>
{% endif %}
{% endfor %}
