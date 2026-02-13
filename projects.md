---
layout: page
title: Projects
permalink: /projects/
---

<div class="card-grid">
{% for project in site.projects %}
  <div class="card">
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <p>{{ project.excerpt | strip_html | truncate: 120 }}</p>
  </div>
{% endfor %}
</div>
