---
layout: archive
permalink: /publications/year-archive/
title: "Posts by Year"
---

{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'"  %}
{% for year in postsByYear %}
  <h2 id="{{ year.name | slugify }}" class="archive__subtitle">{{ year.name }}</h2>
  {% for post in year.items %}
     {% include tag-list.html %}
  {% endfor %}
{% endfor %}
