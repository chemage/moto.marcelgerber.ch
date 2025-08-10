---
layout: home
title: "Homepage"
permalink: /
author_profile: true
---

Bienvenue sur ma page d'affaires à vendre.

## Mes équipements moto à vendre

<div class="cards">
{% for item in site.gear %}
  <article class="card">
	<a href="{{ item.url }}">
		<h3 class="card-title">{{ item.title }}</h3>
    </a>
	<div class="card-content">
	<p class="card-size">{{ item.size }}</p>
	<p class="card-price">{{ item.price }}</p>
	</div>
	<a href="{{ item.url }}">
    	<img class="card-image" src="{{ item.image }}" alt="{{ item.title }}">
    </a>
  </article>
{% endfor %}
</div>

