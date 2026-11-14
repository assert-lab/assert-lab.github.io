---
layout: default
description: "AS²ERT Lab (AI for Safe Software Engineering and Testing) at The University of Texas at Dallas, led by Dr. Soneya Binta Hossain."
---

<section class="home-top2">
  <div class="wrap home-grid">

    <div class="home-col">
      <h1 class="hero-title">AS²ERT Lab</h1>
      <p class="hero-sub"><strong>A</strong>I for <strong>S</strong>afe <strong>S</strong>oftware <strong>E</strong>nginee<strong>r</strong>ing and <strong>T</strong>esting</p>
      <ul class="home-icons" aria-label="Contact and profiles">
        {% for link in site.author.links %}{% if link.url %}
        <li><a href="{{ link.url }}" data-label="{{ link.label }}" aria-label="{{ link.label }}" title="{{ link.label }}"></a></li>
        {% endif %}{% endfor %}
      </ul>
      <div class="home-bio">
    

<p class="home-message">At the AS²ERT Lab, we study how to make <strong>software more reliable</strong> as systems grow increasingly complex and AI takes on a greater role in software development. Our research brings together <strong>software testing, formal verification, and artificial intelligence</strong> to understand software behavior, find faults, and develop stronger methods for establishing correctness. We work across <strong>traditional software, autonomous AI agents, and quantum computing</strong>, addressing fundamental challenges in how software is <strong>tested, verified, and trusted</strong>.</p>

        <p class="home-explore">Explore our <a href="{{ '/project/' | relative_url }}">research areas</a>, <a href="{{ '/publications/' | relative_url }}">publications</a>, and <a href="{{ '/team/' | relative_url }}">team</a>.</p>
      </div>
    </div>

    <div class="home-side">
      <aside class="hire-card" aria-label="Join the lab">
        <p class="hire-card-title">Join our lab</p>
        <p>We’re hiring Ph.D. students interested in AI, software engineering, and quantum computing.</p>
        <p><a class="hire-cta" href="{{ '/join/' | relative_url }}">Explore opportunities →</a></p>
      </aside>

      <aside class="home-recent" aria-label="Recent news">
        <h2>Recent News</h2>
        <ul>
          {% for item in site.data.news limit: 7 %}
          <li><strong>{{ item.date }}</strong> {{ item.short | default: item.text }}</li>
          {% endfor %}
        </ul>
        <p class="home-more"><a href="{{ '/news/' | relative_url }}">All news →</a></p>
      </aside>
    </div>

  </div>
</section>

<section class="home-research">
  <div class="wrap">
    <div class="home-research-head">
      <h2>Research</h2>
      <a href="{{ '/project/' | relative_url }}">All research areas →</a>
    </div>

    <div class="rgroups">
      {% for g in site.data.research_groups %}
      <article class="rgroup">
        <img class="rgroup-fig" src="{{ '/assets/images/' | append: g.figure | relative_url }}" alt="" loading="lazy">
        <div class="rgroup-body">
          <h3>{{ g.title }}</h3>
          <div class="tags">
            {% assign areas = site.data.pub_areas | where: "group", g.key %}
            {% for a in areas %}
            {% assign items = site.data.publications | where: "area", a.key %}
            {% for p in items %}
            {% assign u = p.tag_url | default: p.links[0].url %}
            {% if u %}<a class="tag{% if p.status %} tag-ongoing{% endif %}" href="{{ u }}" title="{{ p.title | escape }}">{{ p.tag }}</a>{% else %}<span class="tag tag-static" title="{{ p.title | escape }}">{{ p.tag }}</span>{% endif %}
            {% endfor %}
            {% endfor %}
          </div>
        </div>
      </article>
      {% endfor %}
    </div>
  </div>
</section>
