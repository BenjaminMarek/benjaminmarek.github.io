---
layout: default
---

Hi, I’m Benjamin Marek. This site collects short analytical essays on economics, politics, and international affairs.

### Recent Essays

{% for post in site.posts %}
{% if post.categories != review %}
- [{{ post.title }}]({{ post.url }}) <small>({{ post.date | date: "%B %Y" }})</small>
{% endif %}
{% endfor %}
