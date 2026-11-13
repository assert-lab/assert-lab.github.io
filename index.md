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
        <strong><a href="{{ '/PI/' | relative_url }}">Dr. Soneya Binta Hossain</a></strong><br>
        Assistant Professor, Department of Computer Science<br>
        The University of Texas at Dallas<br>
        <strong>Email:</strong> <a href="mailto:{{ site.email }}">{{ site.email }}</a>
      </address>

      <div class="home-call">
        <p>We are hiring PhD students and offering remote internships. If you are interested, <a href="mailto:{{ site.email }}">send me an email</a>.</p>
      </div>

      <div class="home-bio">
        <p>Howdy! I lead the AS²ERT Lab at the University of Texas at Dallas. My research focuses on verification and validation of both classical and quantum software systems. We combine AI with established software engineering techniques to improve software correctness checking and ensure reliability, and we study the failure modes of AI-based development tools.</p>

        <p>I received my Ph.D. and M.S. in Computer Science from the University of Virginia, advised by <a href="https://matthewbdwyer.github.io">Prof. Matthew Dwyer</a>, and my B.Sc. from the Bangladesh University of Engineering and Technology (BUET).</p>

        <p>Our work is organized into a few research areas, from test oracles to quantum software assurance. See the <a href="{{ '/project/' | relative_url }}">research areas</a>, <a href="{{ '/publications/' | relative_url }}">publications</a>, and <a href="{{ '/team/' | relative_url }}">people</a>. Undergraduates join the lab through UTD’s RIDE (Research, Inquiry, Design Experience) program.</p>
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
