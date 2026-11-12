---
layout: default
title: "Publications"
permalink: /publications/
description: "Peer-reviewed publications from the AS²ERT Lab and Dr. Soneya Binta Hossain."
---

{% include page-head.html eyebrow="AS²ERT Lab" title="Publications" %}

<div class="wrap">
  <p class="pub-intro">Peer-reviewed publications. A full list is available on <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&amp;hl=en">Google Scholar</a>.</p>

  <div class="page-body">
    {% assign groups = site.data.publications | group_by: "year" %}
    {% for group in groups %}
    <section class="year-block" id="{{ group.name }}">
      <h2 class="year-label">{{ group.name }}</h2>
      <div class="pub-group">
        {% for p in group.items %}
        <article class="pub">
          <h3 class="pub-title">{{ p.title | escape }}</h3>
          <p class="pub-authors">{% for a in p.authors %}{% if a == site.pi_name %}<strong>{{ a }}</strong>{% else %}{{ a }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}</p>
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
