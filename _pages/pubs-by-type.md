---
layout: single
title: "Publications by type" 
permalink: /publications/pubs-by-type/
author_profile: true
toc: true
toc_label: "Pub Types"
---

{% include base_path %}

{% include group-by-array collection=site.posts field="categories" %}


<section class="page__content" itemprop="text" markdown="1">


This is a list of my publications organised by venue types.
{: .text-justify}

</section>

<h2 class="archive__subtitle" id="journals">Journals</h2>

<ul>
  {% for post in site.categories.journal %}
    {% if post.url %}
        <li>{{ post.title }} {{ post.excerpt }}</li>
    {% endif %}
  {% endfor %}
</ul>

<h2 class="archive__subtitle" id="conferences">Conferences and Workshops</h2>

<ul>
  {% for post in site.categories.conference %}
    {% if post.url %}
        <li>{{ post.title }}</li>
    {% endif %}
  {% endfor %}
</ul>

<h2 class="archive__subtitle" id="contributions">Book Contributions</h2>

<ul>
  {% for post in site.categories.book-contribution %}
    {% if post.url %}
        <li>{{ post.title }}</li>
    {% endif %}
  {% endfor %}
</ul>

<h2 class="archive__subtitle" id="edited">Edited Volumes</h2>

<ul>
  {% for post in site.categories.edited-volume %}
    {% if post.url %}
        <li>{{ post.title }}</li>
    {% endif %}
  {% endfor %}
</ul>



<section class="page__content cf" itemprop="text" markdown="1">

> "can add quote here"

<cite>famous author</cite> (date-date) 
{: .small}

</section>
