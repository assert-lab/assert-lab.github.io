---
layout: default
title: "Publications"
permalink: /publications/
description: "Published work from the AS²ERT Lab and Dr. Soneya Binta Hossain, by year, venue, and track."
---

{% include page-head.html eyebrow="AS²ERT Lab" title="Publications" %}

<div class="wrap">
  <p class="pub-intro">Published, peer-reviewed work. A full list is available on <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&amp;hl=en">Google Scholar</a>.</p>

  <div class="page-body">
    <ol class="pub-table">
      {% assign published = site.data.publications | where: "published", true %}
      {% for p in published %}
      {% assign paper = nil %}
      {% for l in p.links %}{% if l.label == "Paper" or l.label == "arXiv" %}{% unless paper %}{% assign paper = l.url %}{% endunless %}{% endif %}{% endfor %}
      {% assign yr = p.year | append: "" %}
      {% assign parts = p.short | split: ", " %}
      <li class="pub-row">
        <div class="pub-meta">
          <span class="pub-year">{{ p.year }}</span>
          <span class="pub-venue-name">{{ parts[0] | remove: yr | strip | escape }}</span>
          {% if parts[1] %}<span class="pub-track">{{ parts[1] | escape }}</span>{% endif %}
        </div>
        <div class="pub-name">{% if paper %}<a href="{{ paper }}">{{ p.title | escape }}</a>{% else %}{{ p.title | escape }}{% endif %}</div>
      </li>
      {% endfor %}
    </ol>
  </div>
</div>
