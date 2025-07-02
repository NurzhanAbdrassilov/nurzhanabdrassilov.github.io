---
layout: projects
title: "projects"
permalink: /projects/
author_profile: false 
sidebar:
  disable: true
---

<div class="projects-page-wrapper">
  <h1 class="page__title">{{ page.title }}</h1>

  <div class="projects-grid">
    {% for project in site.projects %}
    <div class="project-card">
      <h3>{{ project.title }}</h3>
      <p>{{ project.excerpt | markdownify }}</p>
      <a href="{{ project.url | relative_url }}">Read more</a>
    </div>
    {% endfor %}
  </div>
</div>