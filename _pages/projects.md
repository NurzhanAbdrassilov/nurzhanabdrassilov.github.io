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
  grid-template-columns: repeat(3, 1fr); /* 3 columns */
  gap: 2rem;
  width: 100%;
  max-width: 1600px; /* try 1400–1600px for comfort */
  margin-left: auto;
  margin-right: auto;
  margin-top: 2rem;
  padding: 0 2rem;
}

.project-card {
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 1.5rem;
  background-color: #fafafa;
  box-shadow: 2px 2px 6px rgba(0, 0, 0, 0.06);
  transition: transform 0.2s ease;
}

.project-card:hover {
  transform: translateY(-4px);
}

.project-card h3 {
  margin-top: 0;
}

.project-card ul {
  padding-left: 1.2rem;
  margin-bottom: 0;
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

