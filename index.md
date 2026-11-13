---
layout: default
description: "AS²ERT Lab (AI for Safe Software Engineering and Testing) at The University of Texas at Dallas, led by Dr. Soneya Binta Hossain."
---

<section class="home-head">
  <div class="wrap">
    <h1 class="hero-title">AS²ERT Lab</h1>
    <p class="hero-sub">AI for Safe Software Engineering and Testing</p>

    <address class="home-contact">
      Department of Computer Science<br>
      The University of Texas at Dallas<br>
      Led by <a href="{{ '/PI/' | relative_url }}">Dr. Soneya Binta Hossain</a><br>
      <strong>Email:</strong> <a href="mailto:{{ site.email }}">{{ site.email }}</a>
    </address>
  </div>
</section>

<section class="hire-band">
  <div class="wrap">
    <div class="hire-panel">
      <p>
        <strong>Join Our Lab!</strong>
        We are hiring PhD students who are passionate about AI, Software Engineering and Quantum Computing.
        <a class="hire-cta" href="{{ '/join/' | relative_url }}" style="color:#ffffff;">Explore opportunities →</a>
      </p>
    </div>
  </div>
</section>

<section class="home-main2">
  <div class="wrap home-grid">

    <div class="home-col">
      <div class="home-bio">
        <p class="home-message">As AI begins to write code, make decisions, and operate increasingly complex systems, the fundamental challenge of software engineering is establishing what we can trust. At the AS²ERT Lab, we aim to redefine how software correctness is established. We advance software testing, formal verification, and trustworthy AI to uncover hidden failures, reason about intended behavior, and prevent errors before they cause harm. From traditional software to autonomous agents and quantum computing, our ambition is to make software trustworthiness something we can systematically establish, measure, and verify.</p>

        <p class="home-explore">Explore our <a href="{{ '/project/' | relative_url }}">research areas</a>, <a href="{{ '/publications/' | relative_url }}">publications</a>, and <a href="{{ '/team/' | relative_url }}">people</a>.</p>
      </div>
    </div>

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
</section>

<section class="home-research">
  <div class="wrap">
    <div class="home-research-head">
      <h2>Research</h2>
      <a href="{{ '/project/' | relative_url }}">All research areas →</a>
    </div>

    <div class="rgrid">
      {% for a in site.data.pub_areas %}
      {% assign items = site.data.publications | where: "area", a.key %}
      <article class="rcard{% unless a.figure %} rcard-nofig{% endunless %}">
        {% if a.figure %}<img src="{{ '/assets/images/' | append: a.figure | relative_url }}" alt="" loading="lazy">{% endif %}
        <div>
          <h3>{{ a.title }}</h3>
          <p>{{ a.tagline }}</p>
          <div class="tags">
            {% for p in items limit: 3 %}
            {% assign u = p.tag_url | default: p.links[0].url %}
            {% if u %}<a class="tag{% if p.status %} tag-ongoing{% endif %}" href="{{ u }}" title="{{ p.title | escape }}">{{ p.tag }}</a>{% else %}<span class="tag tag-static" title="{{ p.title | escape }}">{{ p.tag }}</span>{% endif %}
            {% endfor %}
          </div>
        </div>
      </article>
      {% endfor %}
    </div>
  </div>
</section>
