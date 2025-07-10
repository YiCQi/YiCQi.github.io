---
layout: archive
title: "My Cats"
permalink: /cats/
author_profile: true
---

{% for cat in site.cats %}
  <h2><a href="{{ cat.url }}">{{ cat.name }}</a></h2>
  <p>{{ cat.content | markdownify | truncatewords: 30 }}</p>
{% endfor %}
