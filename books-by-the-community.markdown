---
title: Books by the Community
date: 2020-07-29 00:38:00 -04:00
permalink: "/books"
layout: archive
---

<ul>
  {% for book in site.book %}
    {% assign book-posts = site.posts | reverse | where: 'book', page.title %}
    {% if book-posts.size > 0 %}
      <li><a href="#{{ book.url }}">{{ book.title }} ({{ book-posts.size }})</a></li>
    {% endif %}
    {% assign book-posts = nil %}
  {% endfor %}
</ul>

{% for book in site.books %}
  {% assign book-posts = site.posts | reverse | where: 'book', book.title %}
  {% if book-posts.size > 0 %}
    <h3>{{ book.title }}</h3>
    <p>{{ book.content }}</p>
    <ul>
      {% for post in book-posts %}
      <li><time datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">{{ post.date | date: "%B %d, %Y" }}</time>:
        <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  {% endif %}
  {% assign book-posts = nil %}
{% endfor %}