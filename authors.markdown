---
title: Authors
date: 2020-07-29 00:22:00 -04:00
permalink: "/authors"
layout: archive
---

<ul>
  {% for author in site.authors %}
    <li><a href="{{ author.url }}">{{ author.title }}</a></li>
  <blockquote>{{ author.excerpt }}</blockquote>
  {% endfor %}
</ul>
