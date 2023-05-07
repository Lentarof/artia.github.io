---
layout: default
title: Galería
---

<h1>Galería</h1>

<div class="gallery">
  {% for image in site.static_files %}
    {% if image.path contains 'galeria/' %}
      <img src="{{ site.baseurl }}/{{ image.path }}" alt="{{ image.name }}">
    {% endif %}
  {% endfor %}
</div>
