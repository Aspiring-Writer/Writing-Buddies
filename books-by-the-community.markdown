---
title: Books by the Community
permalink: "/books"
layout: archive
---

{% for book in site.books %}
<h2><a href="{{ book.url }}">{{ book.title }}</a></h2>
<p><a href="{{ author.url }}">{{ book.author }}</a></p>
<p>{{ book.content }}</p>
{% endfor %}
