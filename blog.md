---
layout: page
title: Blog
permalink: /blog/
---

<div class="card-grid">
{% for post in site.posts %}
  <div class="card">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
    <small>{{ post.date | date: "%b %d, %Y" }}</small>
  </div>
{% endfor %}
</div>
