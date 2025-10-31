---
layout: default
---

## Recent Thoughts

<div style="max-height: 80vh; overflow-y: auto; padding-right: 1em;">

  {% for post in site.posts %}
    {% unless post.categories contains "review" %}
      <article style="margin-bottom: 3em; border-bottom: 1px solid #ddd; padding-bottom: 2em;">
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p class="byline" style="font-style: italic; color: #666; margin-top: -1em; margin-bottom: 1em;">
          by {{ post.author | default: site.author }} · {{ post.date | date: "%B %-d, %Y" }}
        </p>
        {{ post.content }}
      </article>
    {% endunless %}
  {% endfor %}

</div>
