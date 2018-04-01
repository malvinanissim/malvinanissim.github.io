---
layout: archive
title: "Publications by topic"
permalink: /publications/pubs-by-tags/
---

<!-- {% include base_path %} -->

{% include group-by-array.html collection=site.posts field='tags' %}

<ul>
  {% for tag in group_names %}
    {% assign posts = group_items[forloop.index0] %}
    <li>
      <h2>{{ tag }}</h2>
      <ul>
        {% for post in posts %}
        <li>
          {{ post.title }}
        </li>
        {% endfor %}
      </ul>
    </li>
  {% endfor %}
</ul>



