---
layout: single
title: "projects"
permalink: /projects/
author_profile: false   
sidebar:
  disable: true
---

<style>
.page__inner-wrap {
  max-width: none !important;
  padding: 0 !important;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
  max-width: 1600px;
  margin: 2rem auto 0 auto;
  padding: 0 2rem;
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

