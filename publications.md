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
    <section class="year-block" id="{{ group.name }}">
      <h2 class="year-label">{{ group.name }}</h2>
      <ol class="pub-table">
        {% for p in group.items %}
        {% assign yr = p.year | append: "" %}
        {% assign parts = p.short | split: ", " %}
        <li class="pub-row">
          <div class="pub-meta">
            <span class="pub-venue-name">{{ parts[0] | remove: yr | strip | escape }}</span>
            {% if parts[1] %}<span class="pub-track">{{ parts[1] | escape }}</span>{% endif %}
          </div>
          <div class="pub-name">{{ p.title | escape }}{% if p.authors %}
            <span class="pub-authors">{% for a in p.authors %}{% if a == site.pi_name %}<strong>{{ a | escape }}</strong>{% else %}{{ a | escape }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}</span>{% endif %}
            <span class="pub-resources"><span class="pub-resgroup">{% for l in p.links %}{% unless l.label == "GitHub" or l.label == "Artifact" or l.label == "Poster" %}{% if l.url contains "http" %}<span class="pub-res"><a href="{{ l.url }}" aria-label="{{ l.label | escape }}: {{ p.title | escape }}">{{ l.label | escape }}</a></span>{% endif %}{% endunless %}{% endfor %}</span><span class="pub-resgroup">{% for l in p.links %}{% if l.label == "GitHub" or l.label == "Artifact" or l.label == "Poster" %}{% if l.url contains "http" %}<span class="pub-res"><a href="{{ l.url }}" aria-label="{{ l.label | escape }}: {{ p.title | escape }}">{{ l.label | escape }}</a></span>{% endif %}{% endif %}{% endfor %}</span></span></div>
        </li>
        {% endfor %}
      </ol>
    </section>
    {% endfor %}
  </div>
</div>
