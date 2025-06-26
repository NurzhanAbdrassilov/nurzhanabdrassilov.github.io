---
layout: archive
title: "projects"
permalink: /projects/
author_profile: false
---

{% include base_path %}


{% for post in site.projects %}
  {% include archive-single.html %}
{% endfor %}

