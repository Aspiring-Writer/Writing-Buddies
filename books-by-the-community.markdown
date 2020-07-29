---
title: Books by the Community
permalink: "/books"
layout: archive
---

<ul>
  {% for book in site.books %}
    <li><a href="{{ book.url }}">{{ book.title }}</a></li>
  <blockquote>{{ book.content }}</blockquote>
  {% endfor %}
</ul>
