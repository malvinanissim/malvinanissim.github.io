---
layout: single
title: "Publications by topic"
permalink: /publications/pubs-by-tags/
toc: true
toc_label: "Tags"
---

{% include group-by-array collection=site.posts field="tags" %}
{% include tag-list.html % }


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
  

