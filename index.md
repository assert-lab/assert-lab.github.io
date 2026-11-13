---
layout: default
description: "AS²ERT Lab (AI for Safe Software Engineering and Testing) at The University of Texas at Dallas, led by Dr. Soneya Binta Hossain."
---

<div class="hire-bar">
  <div class="wrap hire-inner">
    <p><strong>We are hiring PhD students.</strong> Remote internships are also available.</p>
    <a class="hire-link hire-mail" href="mailto:{{ site.email }}">Get in touch</a>
  </div>
</div>

<section class="home-top">
  <div class="wrap home-grid">

    <div class="home-col">
      <h1 class="hero-title">AS²ERT Lab</h1>
      <p class="hero-sub">AI for Safe Software Engineering and Testing</p>

      <p class="home-lede">Howdy! Welcome to the AS²ERT Lab at the University of Texas at Dallas. We develop methods, datasets, and benchmarks that make software, classical and quantum, more trustworthy, reliable, and safe.</p>
      <p class="home-led">Led by <a href="{{ '/PI/' | relative_url }}">Dr. Soneya Binta Hossain</a>, Assistant Professor of Computer Science at UTD.</p>

      <div class="actions">
        <a class="btn btn-primary" href="{{ '/project/' | relative_url }}">Our research</a>
        <a class="btn" href="{{ '/team/' | relative_url }}">Meet the team</a>
      </div>

      <div class="home-block">
        <h2>Undergraduate research</h2>
        <p>Through UTD’s RIDE (Research, Inquiry, Design Experience) program, undergraduates work on carefully scoped projects and grow into independent researchers.</p>
        <ul class="home-ride">
          <li><span>RIDE 033</span> Trustworthy AI in Software Testing</li>
          <li><span>RIDE 041</span> Trustworthy AI in Software Engineering</li>
          <li><span>RIDE 045</span> Trustworthy AI in Quantum Software Engineering</li>
        </ul>
      </div>
    </div>

    <aside class="home-news" aria-label="News">
      <h2>News</h2>
      <ul class="home-news-list">
        {% for item in site.data.news limit: 6 %}
        <li>
          <span class="home-news-date">{{ item.date }}</span>
          <span class="home-news-text">{{ item.short | default: item.text }}</span>
        </li>
        {% endfor %}
      </ul>
      <p class="home-more"><a href="{{ '/news/' | relative_url }}">All news →</a></p>
    </aside>

  </div>
</section>
