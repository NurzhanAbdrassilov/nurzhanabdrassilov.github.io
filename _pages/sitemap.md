---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of core pages and blog posts on this site.

---

<h2>Pages</h2>
<ul>
  {% assign allowed_paths = "/projects/,/research/,/resume/,/sitemap/,/blog/" | split: "," %}
  {% for page in site.pages %}
    {% if allowed_paths contains page.url %}
      <li><a href="{{ page.url | relative_url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>


<h2>Projects</h2>
<ul>
  {% for item in site.projects %}
    <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
  {% endfor %}
</ul>

<h2>Blog Posts</h2>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> – {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>

