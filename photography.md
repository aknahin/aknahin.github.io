---
layout: page
title: Photography
description: >
  Moments I've captured away from the lab.
redirect_from:
  - /photography.html
---

{% assign photos = site.static_files | where_exp: "f", "f.path contains '/assets/gallery/'" | sort: "path" %}
<div class="photo-mosaic"><div class="photo-grid">
{% for photo in photos %}
  <a href="{{ photo.path | relative_url }}" class="photo">
    <img src="{{ photo.path | relative_url }}" alt="Photograph {{ forloop.index }}" loading="lazy" decoding="async">
  </a>
{% endfor %}
</div></div>
