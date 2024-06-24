---
layout: default
title: Home
---

# Welcome to My ML/AI Portfolio

This site showcases my journey and projects in Machine Learning and Artificial Intelligence. Below are some of my key projects.

<section class="featured-section">
  <h2>Featured Projects</h2>
  <p>Explore some of my most prominent work in the field of ML/AI. Click on a project to learn more about its details, technologies used, and the outcomes achieved.</p>
</section>

<div class="project-list">
  {% for project in site.projects %}
    <div class="post-card">
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
