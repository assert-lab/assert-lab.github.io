---
layout: default
title: "Publications"
permalink: /publications/
description: "Publications from the AS²ERT Lab and Dr. Soneya Binta Hossain on software testing, specifications, trustworthy AI, debugging, and quantum software assurance."
---

{% include page-head.html eyebrow="AS²ERT Lab" title="Publications" %}

<div class="wrap">
  <p class="pub-intro">Peer-reviewed papers, preprints, and a dissertation, grouped by research area. A full list is available on <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&amp;hl=en">Google Scholar</a>.</p>

  <nav class="pub-nav" aria-label="Research areas">
    {% for a in site.data.pub_areas %}
    <a href="#{{ a.key }}">{{ a.title }}</a>
    {% endfor %}
  </nav>

  {% for a in site.data.pub_areas %}
  {% assign items = site.data.publications | where: "area", a.key %}
  {% if items.size != 0 or a.show_empty %}
  <section class="pub-area" id="{{ a.key }}">
    <div class="pub-area-side">
      <h2>{{ a.title }}</h2>
      <p>{{ a.blurb }}</p>
      {% if a.figure %}<img class="pub-fig" src="{{ '/assets/images/' | append: a.figure | relative_url }}" alt="{{ a.alt | escape }}" loading="lazy">{% endif %}
    </div>
    <div class="pub-list">
      {% for p in items %}
      <article class="pub">
        <h3 class="pub-title">{{ p.title | escape }}{% if p.status %}<span class="pub-status">{{ p.status }}</span>{% endif %}</h3>
        {% if p.authors %}<p class="pub-authors">{% for au in p.authors %}{% if au == site.pi_name %}<strong>{{ au }}</strong>{% else %}{{ au }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}</p>{% endif %}
        <p class="pub-venue">{{ p.venue | escape }} (<span class="short">{{ p.short | escape }}</span>){% if p.note %} <span class="pub-note">· {{ p.note | escape }}</span>{% endif %}</p>
        {% if p.links %}
        <p class="pub-links">{% for l in p.links %}<a href="{{ l.url }}">{{ l.label }}</a>{% endfor %}</p>
        {% endif %}
      </article>
      {% endfor %}
      {% if items.size == 0 %}<p class="pub-empty">{{ a.empty_note }}</p>{% endif %}
    </div>
  </section>
  {% endif %}
  {% endfor %}

  <p class="endnote">For the complete list of publications, please visit the <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&amp;hl=en">Google Scholar</a> profile.</p>
</div>
