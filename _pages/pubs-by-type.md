---
layout: archive
title: "Pubs" 
permalink: /publications/pubs-by-type/
---

{% include base_path %}

{% include group-by-array collection=site.posts field="categories" %}

{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}

<section class="page__content" itemprop="text" markdown="1">


This list of publications __understanding software__
In particular, in my PhD research I
harnessed the knowledge about software systems incorporated in existing test
cases to drive the __automatic generation__ of new complex test cases at a low
{: .text-justify}

</section>

<!--
{% include group-by-array collection=site.posts field="categories" %}

{% for post in site.posts %}
{% include archive-single.html %}
{% endfor %}
-->

<h3 class="archive__subtitle">Journals</h3>

<div class="cf"> 
<div class="grid__wrapper">

{% for category in group_names %}
  <!-- only research -->
  {% if category contains site.journal %}
    {% assign posts = group_items[forloop.index0] %}
    {% for post in posts %}
    {% include archive-single.html type="grid" %}
    {% endfor %}
  {% endif %}
{% endfor %}

</div>
</div>



<section class="page__content cf" itemprop="text" markdown="1">

> "can add quote here"

<cite>famous author</cite> (date-date) 
{: .small}

</section>
