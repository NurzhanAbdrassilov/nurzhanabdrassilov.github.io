---
layout: default
title: "projects"
permalink: /projects/
author_profile: false
sidebar:
  disable: true
---

<div class="projects-page-wrapper">
  <div class="projects-grid">
    <h1 class="page__title">{{ page.title }}</h1>

    {% for project in site.projects %}
    <div class="project-card">
      <h3>{{ project.title }}</h3>
      <p>{{ project.excerpt | markdownify }}</p>
      <a href="{{ project.url | relative_url }}">Read more</a>
    </div>
    {% endfor %}
  </div>
</div>
