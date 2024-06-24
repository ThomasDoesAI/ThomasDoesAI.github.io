---
layout: default
title: Home
---

# Welcome to My ML/AI Portfolio

This site showcases my journey and projects in Machine Learning and Artificial Intelligence. Below are some of my key projects.

{% for project in site.projects %}
## [{{ project.title }}]({{ project.url }})
{{ project.excerpt }}
{% endfor %}
