---
layout: default
title: Home
---

# Welcome to My ML/AI Portfolio

{% for collection in site.collections %}
### Collection: {{ collection.label }}
{% endfor %}

{% for project in site.projects %}
## [{{ project.title }}]({{ project.url }})
{{ project.excerpt }}
{% endfor %}
