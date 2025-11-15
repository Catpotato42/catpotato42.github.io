---
layout: page
title: "Portfolio"
permalink: /portfolio/
---

{% for item in site.portfolio %}
  <article class="portfolio-item">
    <a href="{{ item.url }}">
      {% if item.thumbnail %}
        <img src="{{ item.thumbnail }}" alt="{{ item.title }}" class="thumb">
      {% endif %}
      <h2>{{ item.title }}</h2>
    </a>
  </article>
{% endfor %}
