---
layout: default
title: Home
---

# Welcome to My ML/AI Portfolio

This site showcases my journey and projects in Machine Learning and Artificial Intelligence. Below are some of my key projects.

<h2>Projects Collection:</h2>
<ul>
{% for project in site.projects %}
  <li>{{ project.title }} - {{ project.url }}</li>
{% else %}
  <li>No projects found. Ensure projects have the correct front matter and are located in the projects directory.</li>
{% endfor %}
</ul>

<h2>All Site Collections:</h2>
<ul>
{% for collection in site.collections %}
  <li>{{ collection.label }}: {{ collection.docs | size }} items</li>
{% endfor %}
</ul>
