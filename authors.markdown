---
title: Authors
date: 2020-07-29 00:22:00 -04:00
layout: archive
permalink: /authors
---

<ul>
  {% for author in site.authors %}
    <li><a href="{{ author.url }}">{{ author.title }}</a></li>
  {% endfor %}
</ul>
