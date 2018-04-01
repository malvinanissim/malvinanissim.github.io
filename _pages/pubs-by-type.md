---
layout: archive
title: "Pubs" 
permalink: /publications/pubs-by-type/
toc: true
---

{% include base_path %}

{% include group-by-array collection=site.posts field="categories" %}


<section class="page__content" itemprop="text" markdown="1">


This list of publications __understanding software__
In particular, in my PhD research I
harnessed the knowledge about software systems incorporated in existing test
cases to drive the __automatic generation__ of new complex test cases at a low
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




<section class="page__content cf" itemprop="text" markdown="1">

> "can add quote here"

<cite>famous author</cite> (date-date) 
{: .small}

</section>
