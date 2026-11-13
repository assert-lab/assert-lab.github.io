---
layout: default
description: "AS²ERT Lab (AI for Safe Software Engineering and Testing) at The University of Texas at Dallas, led by Dr. Soneya Binta Hossain."
---

<div class="hire-bar">
  <div class="wrap hire-inner">
    <p><strong>We are hiring PhD students.</strong> Remote internships are also available, particularly for international students.</p>
    <a class="hire-link" href="#join">Read more</a>
    <a class="hire-link hire-mail" href="mailto:{{ site.email }}">Get in touch</a>
  </div>
</div>

<section class="home-hero">
  <div class="wrap home-hero-grid">

    <div class="home-hero-copy">
      <h1 class="hero-title">AS²ERT Lab</h1>
      <p class="hero-sub">AI for Safe Software Engineering and Testing</p>

      <p class="home-lede">Howdy! Welcome to the <strong>AS²ERT Lab</strong> (<strong>AI for Safe Software Engineering and Testing</strong>) at the University of Texas at Dallas. We can hardly go a single day without relying on software — in the apps we use, the systems we build, and the infrastructure that supports our everyday lives. As software becomes more deeply woven into society, it becomes increasingly important to make these systems trustworthy, reliable, and safe.</p>

      <p class="home-body">At the <strong>AS²ERT Lab</strong>, we see trustworthy software as a full-lifecycle challenge. We build cost-effective and robust methods that help developers improve software reliability and trustworthiness; study how modern AI methods — including large language models and agentic systems — can be used responsibly across testing, debugging, fault localization, and repair; and create high-quality datasets and benchmarks that help the community measure real progress in trustworthy software engineering. Our work spans both classical and quantum software systems.</p>

      <div class="actions">
        <a class="btn btn-primary" href="{{ '/project/' | relative_url }}">Explore our research</a>
        <a class="btn" href="{{ '/team/' | relative_url }}">Meet the team</a>
      </div>
    </div>

    <figure class="home-portrait">
      <div class="portrait-frame">
        <img src="{{ '/assets/images/soneya-b.jpg' | relative_url }}" alt="Dr. Soneya Binta Hossain">
      </div>
      <figcaption>The AS²ERT Lab is founded by <a href="{{ '/PI/' | relative_url }}"><strong>Dr. Soneya Binta Hossain</strong></a>, Assistant Professor of Computer Science at UTD.</figcaption>
    </figure>

  </div>
</section>

<section class="home-main">
  <div class="wrap home-grid">

    <div class="home-col">

      <div class="home-block">
        <h2>Our research</h2>
        <p>Our work spans software testing and test oracles, software specifications, trustworthy AI and agents, debugging and repair, and quantum software assurance, with the datasets, benchmarks, and tools that support them.</p>
        <p class="home-more"><a href="{{ '/project/' | relative_url }}">See the research areas and papers →</a></p>
      </div>

      <div class="home-block" id="join">
        <h2>Join the lab</h2>
        <p>The AS²ERT Lab is looking for graduate students who are excited about software engineering research. If you are interested, we encourage you to take a look at our recent work and reach out with your thoughts on what current approaches miss and where the field could go next. Our lab culture values intellectual ownership, high standards, and deep technical engagement, along with open, principled discussion and follow-through. These values are closely aligned with these <a href="https://www.amazon.jobs/content/en/our-workplace/leadership-principles" target="_blank" rel="noopener">principles</a>.</p>
        <p><strong>Remote internships:</strong> We offer remote internship opportunities, particularly for international students. Please reach out via email if interested.</p>
        <p class="home-more"><a href="mailto:{{ site.email }}">{{ site.email }}</a></p>
      </div>

      <div class="home-block">
        <h2>Undergraduate research</h2>
        <p>The AS²ERT Lab is deeply committed to mentoring motivated undergraduate students and helping them grow into confident, independent researchers in Software Engineering. UTD’s <strong>RIDE (Research, Inquiry, Design Experience)</strong> program provides an excellent foundation for introducing undergraduates to research in a structured and supportive environment. Through RIDE, students work on carefully scoped projects that encourage them to ask meaningful research questions, build and evaluate technical solutions, and communicate their findings at a level suitable for scholarly venues.</p>
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
          <span class="home-news-text">{{ item.text }}</span>
        </li>
        {% endfor %}
      </ul>
      <p class="home-more"><a href="{{ '/news/' | relative_url }}">All news and updates →</a></p>
    </aside>

  </div>
</section>
