---
layout: default
title: Home
---

# Welcome to My ML/AI Portfolio

This site showcases my journey and projects in Machine Learning and Artificial Intelligence. Below are some of my key projects.

{% for project in site.projects %}
- **Project Title:** {{ project.title }}
- **Project URL:** {{ project.url }}
- **Project Excerpt:** {{ project.excerpt }}
{% endfor %}

<!-- Additional debug info -->
{% for project in site.projects %}
  <div>
    <h2><a href="{{ project.url }}">{{ project.title }}</a></h2>
    <p>{{ project.content | truncatewords: 30 }}</p>
  </div>
{% else %}
  <p>No projects found. Ensure projects have the correct front matter and are located in the projects directory.</p>
{% endfor %}
