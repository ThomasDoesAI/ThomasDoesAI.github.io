---
layout: default
title: Projects
---

# My Projects

Welcome to my project portfolio. Here, you will find a curated selection of my work in Machine Learning and Artificial Intelligence. Each project includes a detailed description, the technologies used, and the outcomes achieved.

<section class="featured-section">
  <h2>Highlighted Projects</h2>
  <p>Below are some of the highlighted projects I've worked on. Click on any project to learn more about it.</p>
</section>

<div class="project-grid">
  {% for project in site.projects %}
    <div class="project-card">
      <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
      <p>{{ project.excerpt | strip_html | truncatewords: 30 }}</p>
      <a href="{{ project.url }}" class="btn">Read More</a>
    </div>
  {% else %}
    <p>No projects found. Ensure projects have the correct front matter and are located in the _projects directory.</p>
  {% endfor %}
</div>

<footer>
  <p>&copy; {{ site.time | date: '%Y' }} {{ site.title }}. All rights reserved.</p>
</footer>
