---
title: Books by the Community
date: 2020-07-29 00:38:00 -04:00
permalink: "/books"
layout: archive
---

<ul>
  {% for book in site.books %}
    <li><a href="{{ book.url }}">{{ book.title }}</a></li>
  <blockquote>{{ book.content }}</blockquote>
  {% endfor %}
</ul>
