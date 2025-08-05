---
layout: home
title: "Homepage"
permalink: /
author_profile: true
---

Bienvenue sur ma page d'affaires à vendre.

## Mes équipements moto à vendre

{% for item in site.gear %}
- [{{ item.title }}]({{ item.url }}) — {{ item.price }}
{% endfor %}

