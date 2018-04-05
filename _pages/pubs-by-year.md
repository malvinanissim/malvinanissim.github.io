---
layout: single
title: "Publications by year"
permalink: /publications/pubs-by-year/
toc: true
toc_label: "Years"
author_profile: true
---

{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'"  %}
{% for year in postsByYear %}
  <h2 id="{{ year.name | slugify }}" class="archive__subtitle">{{ year.name }}</h2>
  <ul>
  {% for post in year.items %}
  {% if post.url %}
        <li>{{ post.title }} [<span style="background-color:#CC0000;">{{ post.categories }}</span>]</li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}
