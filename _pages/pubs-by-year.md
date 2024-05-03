---
title: "Publications by year"
permalink: /publications/pubs-by-year/
toc_label: "Years"
---

{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'"  %}
{% for year in postsByYear %}
  <h2 id="{{ year.name | slugify }}" class="archive__subtitle">{{ year.name }}</h2>
  <ul>
  {% for post in year.items %}
  {% if post.url %}
        <li>{{ post.title }} [<span style="color:#CC0000;">{{ post.categories }}</span>]</li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}
