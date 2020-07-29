---
title: Plays by the Community
permalink: "/plays/"
layout: archive
---

<div class="tiles">
{% for post in site.categories.plays %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
