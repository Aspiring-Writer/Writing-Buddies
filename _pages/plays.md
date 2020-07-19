---
layout: archive
permalink: /plays/
title: "Plays by the Community"
---

<div class="tiles">
{% for post in site.categories.plays %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
