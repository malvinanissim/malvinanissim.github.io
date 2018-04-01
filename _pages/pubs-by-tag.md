---
layout: archive
title: "Publications by topic"
permalink: /publications/pubs-by-tags/
---

{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  <ul>
  {% for post in posts %}
    {% if post.url %}
        <li>{{ post.title }}</li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}
  

