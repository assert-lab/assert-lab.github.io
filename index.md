---
layout: default
description: "AS²ERT Lab (AI for Safe Software Engineering and Testing) at The University of Texas at Dallas, led by Dr. Soneya Binta Hossain."
---

<section class="home-top">
  <div class="wrap home-grid">

    <div class="home-col">
      <h1 class="hero-title">AS²ERT Lab</h1>
      <p class="hero-sub">AI for Safe Software Engineering and Testing</p>

      <address class="home-contact">
        Department of Computer Science<br>
        The University of Texas at Dallas<br>
        Led by <a href="{{ '/PI/' | relative_url }}">Dr. Soneya Binta Hossain</a><br>
        <strong>Email:</strong> <a href="mailto:{{ site.email }}">{{ site.email }}</a>
      </address>

    
<div class="hire-panel">
  <p>
    <strong>Join Our Lab!</strong>
    We welcome curious and motivated PhD students, undergraduate researchers, and remote collaborators who are passionate about advancing software engineering and trustworthy AI.
    <a href="{{ '/join/' | relative_url }}">Explore opportunities →</a>
  </p>
</div>



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
