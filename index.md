---
layout: default
title: Home
---

# Welcome to My ML/AI Portfolio
This site showcases my journey and projects in Machine Learning and Artificial Intelligence. Below are some of my key projects.

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
{{ post.excerpt }}
{% endfor %}
