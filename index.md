---
layout: home
title: Home
---

Hi, I'm Abdullah

I'm an aspiring SOC analyst, currently a student.

Welcome to my corner of the internet.

## Featured Projects
<div class="card-grid">
{% for project in site.projects limit:2 %}
  <div class="card">
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <p>{{ project.excerpt | strip_html | truncate: 120 }}</p>
  </div>
{% endfor %}
</div>