---
layout: default
title: "Publications"
permalink: /publications/
description: "Published work from the AS²ERT Lab and Dr. Soneya Binta Hossain, by year, venue, and track."
---

{% include page-head.html eyebrow="AS²ERT Lab" title="Publications" %}

<div class="wrap">
  <p class="pub-intro">Published, peer-reviewed work. A full list is available on <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&amp;hl=en">Google Scholar</a>.</p>

  <div class="page-body pubs-page">
    {% assign published = site.data.publications | where: "published", true %}
    {% assign groups = published | group_by: "year" %}
    {% for group in groups %}
    <div class="bib-year" id="{{ group.name }}">
      <ol class="bib-list">
        {% for p in group.items %}
        {% assign yr = p.year | append: "" %}
        {% assign parts = p.short | split: ", " %}
        <li class="bib-item">
          <div class="bib-where"><span>{{ parts[0] | remove: yr | strip | escape }}</span> <span>{{ p.year }}</span></div>
          <div class="bib-main">
            <p class="bib-title">{{ p.title | escape }}</p>
            {% if p.authors %}<p class="bib-authors">{% for a in p.authors %}{% if a == site.pi_name %}<strong>{{ a | escape }}</strong>{% else %}{{ a | escape }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}</p>{% endif %}
            <p class="bib-venue">{% if p.venue %}{{ p.venue | escape }}{% else %}{{ parts[0] | escape }}{% endif %}{% if parts[1] %}, {{ parts[1] | escape }}{% endif %}{% if p.note %} ({{ p.note | escape }}){% endif %}</p>
            <p class="bib-links">{% for l in p.links %}{% unless l.label == "GitHub" or l.label == "Artifact" or l.label == "Poster" or l.label == "arXiv" %}{% if l.url contains "http" %}<a href="{{ l.url }}" aria-label="{{ l.label | escape }}: {{ p.title | escape }}">[{{ l.label | escape }}]</a>{% endif %}{% endunless %}{% endfor %}{% for l in p.links %}{% if l.label == "GitHub" or l.label == "Artifact" or l.label == "Poster" %}{% if l.url contains "http" %}<a href="{{ l.url }}" aria-label="{{ l.label | escape }}: {{ p.title | escape }}">[{{ l.label | escape }}]</a>{% endif %}{% endif %}{% endfor %}</p>
          </div>
        </li>
        {% endfor %}
      </ol>
    </div>
    {% endfor %}
  </div>
</div>
