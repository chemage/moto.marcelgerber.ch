---
layout: home
title: "Homepage"
permalink: /
author_profile: true
---

Bienvenue sur ma page d'affaires à vendre.

{% include dynamic_menu.html %}

## Mes équipements moto à vendre

<div class="cards">
{% for item in site.gear %}
  <article class="card">
    <a href="{{ item.url }}">
      <img class="card-image" src="{{ item.image }}" alt="{{ item.title }}">
      <div class="card-content">
        <h3 class="card-title">{{ item.title }}</h3>
        <p class="card-price">{{ item.price }}</p>
      </div>
    </a>
  </article>
{% endfor %}
</div>

