---
layout: projects
title: "projects"
permalink: /projects/
author_profile: false 
sidebar:
  disable: true
---

<style>
.projects-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 2rem;
  max-width: 1200px;
  margin: 2rem auto;
  padding: 0 1rem;
}

.project-card {
  flex: 0 1 300px;
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 2rem;
  background-color: #fafafa;
  box-shadow: 0 2px 5px rgba(0,0,0,0.08);
  transition: transform 0.2s ease;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.project-card:hover {
  transform: translateY(-4px);
}

.project-card h3 {
  margin-top: 0;
  font-size: 1.2rem;
}

.project-card p {
  font-size: 0.95rem;
  line-height: 1.4;
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



