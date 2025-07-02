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
  max-width: 1000px;
  margin: 2rem auto;
  padding: 0 1rem;
}

.project-card {
  flex: 0 1 calc(33.333% - 2rem); /* 3 per row max */
  max-width: 300px;
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 1.5rem;
  background-color: #fafafa;
  box-shadow: 0 2px 5px rgba(0,0,0,0.08);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  transition: transform 0.2s ease;
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

@media screen and (max-width: 960px) {
  .project-card {
    flex: 0 1 calc(50% - 2rem); /* 2 per row */
  }
}

@media screen and (max-width: 600px) {
  .project-card {
    flex: 0 1 100%; /* 1 per row */
  }
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



