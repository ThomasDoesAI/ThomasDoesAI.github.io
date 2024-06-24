---
layout: post
title: Projects
---

# Projects

Here are some of my key projects:

{% for post in site.projects %}
## [{{ post.title }}]({{ post.url }})
{{ post.excerpt }}
{% endfor %}
