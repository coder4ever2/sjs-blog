---
layout: default
---

# Welcome to SJ's Blog

Thoughts on technology, leadership, and the future.

---

## Recent Posts
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      - <small><em>{{ post.date | date: "%B %d, %Y" }}</em></small>
    </li>
  {% endfor %}
</ul>
