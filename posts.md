---
layout: default
title: Posts
permalink: /posts/
---

# All posts

{% for post in site.posts %}

## [{{ post.title }}]({{ post.url | relative_url }})

<small>{{ post.date | date: "%Y.%m.%d" }}</small>

{{ post.excerpt | strip_html | truncate: 200 }}

---

{% endfor %}
