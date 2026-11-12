---
layout: default
title: "Focus Research Areas"
permalink: /project/
description: "Research areas of the AS²ERT Lab: software testing and test oracles, specifications, trustworthy AI, debugging and repair, and quantum software assurance."
---

{% include page-head.html eyebrow="Research" title="Focus research areas" %}

<div class="wrap">
  <div class="areas">

    {% for a in site.data.pub_areas %}
    <section class="area">
      <div class="area-num">{{ forloop.index | prepend: '0' }}</div>
      <div>
        <h3>{{ a.title }}</h3>
        <p>{{ a.long }}</p>
        <div class="tags">{% include area-tags.html key=a.key %}</div>
      </div>
      {% if a.figure %}<img class="area-fig" src="{{ '/assets/images/' | append: a.figure | relative_url }}" alt="{{ a.alt | escape }}" loading="lazy">{% endif %}
    </section>
    {% endfor %}

    <p class="endnote"><span class="tag tag-static tag-ongoing">Ongoing</span> marks a preprint or work in progress. For the full list, see <a href="{{ '/publications/' | relative_url }}">Publications</a> and <a href="{{ '/news/' | relative_url }}">Lab News</a>.</p>

  </div>
</div>
