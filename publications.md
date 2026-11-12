---
layout: default
title: "Publications"
permalink: /publications/
description: "Publications from the AS²ERT Lab and Dr. Soneya Binta Hossain, by year, venue, and track."
---

{% include page-head.html eyebrow="AS²ERT Lab" title="Publications" %}

<div class="wrap">
  <p class="pub-intro">Peer-reviewed papers, preprints, and a dissertation. A full list is available on <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&amp;hl=en">Google Scholar</a>.</p>

  <div class="page-body">
    {% assign groups = site.data.publications | group_by: "year" %}
    {% for group in groups %}
    <section class="year-block" id="{{ group.name }}">
      <h2 class="year-label">{{ group.name }}</h2>
      <div class="pub-group">
        {% for p in group.items %}
        <article class="pub">
          <h3 class="pub-title">{{ p.title | escape }}{% if p.status %}<span class="pub-status">{{ p.status }}</span>{% endif %}</h3>
          {% if p.authors %}<p class="pub-authors">{% for au in p.authors %}{% if au == site.pi_name %}<strong>{{ au }}</strong>{% else %}{{ au }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}</p>{% endif %}
          <p class="pub-venue">{{ p.venue | escape }} (<span class="short">{{ p.short | escape }}</span>){% if p.note %} <span class="pub-note">· {{ p.note | escape }}</span>{% endif %}</p>
          {% if p.links %}
          <p class="pub-links">{% for l in p.links %}<a href="{{ l.url }}">{{ l.label }}</a>{% endfor %}</p>
          {% endif %}
        </article>
        {% endfor %}
      </div>
    </section>
    {% endfor %}

    <p class="endnote">For the complete list of publications, please visit the <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&amp;hl=en">Google Scholar</a> profile.</p>
  </div>
</div>
