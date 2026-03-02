---
layout: default
title: Home
---

# Latest Blog Posts

{% if site.posts.size > 0 %}
  {% for post in site.posts limit:5 %}

## [{{ post.title }}]({{ post.url }})

*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}

---

  {% endfor %}
{% else %}
No blog posts yet.
{% endif %}
