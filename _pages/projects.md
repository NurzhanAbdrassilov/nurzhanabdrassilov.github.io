---
layout: single
title: "projects"
permalink: /projects/
author_profile: false
sidebar:
  disable: true
---

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.project-card {
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 1rem;
  background-color: #fafafa;
  box-shadow: 2px 2px 5px rgba(0,0,0,0.05);
}

.project-card img {
  max-width: 100%;
  border-radius: 8px;
  margin-top: 0.5rem;
}
</style>

<div class="projects-grid">
  {% for project in site.projects %}
  <div class="project-card">
    <h3>{{ project.title }}</h3>
    <p>{{ project.excerpt | markdownify }}</p>
    <a href="{{ project.url | relative_url }}">Read more</a>
  </div>
  {% endfor %}
</div>

