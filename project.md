---
layout: default
title: "Focus research areas"
permalink: /project/
description: "Research areas of the AS²ERT Lab: software testing and test oracles, specifications, trustworthy AI, debugging and repair, and quantum software assurance."
---

{% include page-head.html eyebrow="Research" title="Focus research areas" %}

<div class="wrap">
  <div class="areas">

    {% for a in site.data.pub_areas %}
    {% assign even = forloop.index | modulo: 2 %}
    <section class="area{% if even == 0 and a.figure %} area-flip{% endif %}">
      <div class="area-text">
        <h2>{{ a.title }}</h2>
        <p>{{ a.long }}</p>
        <div class="tags">{% include area-tags.html key=a.key %}</div>
      </div>
      {% if a.figure %}<img class="area-fig" src="{{ '/assets/images/' | append: a.figure | relative_url }}" alt="{{ a.alt | escape }}" loading="lazy">{% endif %}
    </section>
    {% endfor %}

    <p class="endnote">For the full list, see <a href="{{ '/publications/' | relative_url }}">Publications</a> and <a href="{{ '/news/' | relative_url }}">Lab News</a>.</p>

  </div>
</div>
