---
title: Books by the Community
permalink: "/books"
layout: archive
---

{% include toc.html %}

{% for book in site.books %}
<h2><a href="{{ book.url }}">{{ book.title }}</a></h2>
<p><a href="{{ site.url }}/authors/{{ book.author | slugify }}"><b>Written by {{ book.author }}</b></a></p>
<p>{{ book.content }}</p>
<hr>
{% endfor %}
