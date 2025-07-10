---
layout: archive
title: "Experiences"
permalink: /experiences/
author_profile: true
---

{% include base_path %}

{% assign experiences = site.experiences | sort: "end_date" | reverse %}

{% for exp in experiences %}
  {% include experience-single.html experience=exp %}
{% endfor %}
