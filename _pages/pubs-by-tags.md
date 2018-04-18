---
layout: single
title: "Publications by topic"
permalink: /publications/pubs-by-tags/
toc: true
toc_label: "Topics"
author_profile: true
---

{% assign tags = site.tags | sort %}
{% for tag in tags %}
 <span class="site-tag">
    <a href="/tag/{{ tag | first | slugify }}/"
        style="font-size: {{ tag | last | size  |  times: 4 | plus: 80  }}%">
            {{ tag[0] | replace:'-', ' ' }} ({{ tag | last | size }})
    </a>
</span>
{% endfor %}

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
  

