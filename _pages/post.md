---
title: "Article"
permalink: /posts/
layout: single
author_profile: true
---

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt | strip_html | truncate: 160 }}

[Read more →]({{ post.url }})

---
{% endfor %}