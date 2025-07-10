---
title: "Cats"
permalink: /cats/
layout: archive
author_profile: true
---

<style>
.cat-gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.cat-card {
  width: 200px;
  text-align: center;
}

.cat-card img {
  width: 100%;
  border-radius: 10px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.15);
}
</style>

<div class="cat-gallery">
  {% for cat in site.cats: %}
    <div class="cat-card">
      <a href="{{ cat.url }}">
        {% if cat.image %}
          <img src="{{ cat.image }}" alt="{{ cat.title }}">
        {% endif %}
        <h3>{{ cat.title }}</h3>
      </a>
    </div>
  {% endfor %}
</div>
