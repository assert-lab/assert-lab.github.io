---
layout: default
description: "AS²ERT Lab (AI for Safe Software Engineering and Testing) at The University of Texas at Dallas, led by Dr. Soneya Binta Hossain."
---

<section class="hero">
  <div class="wrap hero-grid">

    <div class="hero-copy">
      <p class="eyebrow">The University of Texas at Dallas</p>
      <h1 class="hero-title">AS²ERT Lab</h1>
      <p class="hero-sub">AI for Safe Software Engineering and Testing</p>

      <p class="lede">
        Howdy! Welcome to the <strong>AS²ERT Lab</strong> (<strong>AI for Safe Software Engineering and Testing</strong>) at the University of Texas at Dallas. We can hardly go a single day without relying on software — in the apps we use, the systems we build, and the infrastructure that supports our everyday lives. As software becomes more deeply woven into society, it becomes increasingly important to make these systems trustworthy, reliable, and safe.
      </p>

      <div class="actions">
        <a class="btn btn-primary" href="{{ '/project/' | relative_url }}">Our research</a>
        <a class="btn" href="#join">Join the lab</a>
      </div>

      <div class="byline">
        <img class="avatar" src="{{ '/assets/images/soneya.jpg' | relative_url }}" alt="">
        <p>The AS²ERT Lab is founded by <a href="{{ '/PI/' | relative_url }}"><strong>Dr. Soneya Binta Hossain</strong></a>, Assistant Professor of Computer Science at UTD.</p>
      </div>
    </div>

    <!-- Decorative only: a nod to the lab's name. Safe to delete this whole block. -->
    <div class="hero-figure" aria-hidden="true">
      <div class="codecard">
        <code><span class="ln">1</span><span class="k">@Test</span></code>
        <code><span class="ln">2</span><span class="k">void</span> trustworthy_software() {</code>
        <code><span class="ln">3</span>    var report = lab.verify(software);</code>
        <code><span class="ln">4</span></code>
        <code class="hl"><span class="ln">5</span>    <span class="a">assert</span>True(report.isCorrect());</code>
        <code class="hl"><span class="ln">6</span>    <span class="a">assert</span>True(report.isSafe());</code>
        <code><span class="ln">7</span>}</code>
      </div>
    </div>

  </div>
</section>

<section class="section">
  <div class="wrap split">
    <div class="split-label">
      <p class="eyebrow">Our approach</p>
      <h2>Trustworthy software as a full-lifecycle challenge</h2>
    </div>
    <div class="split-body">
      <p class="prose-lg">
        At the <strong>AS²ERT Lab</strong>, we see trustworthy software as a full-lifecycle challenge. We build cost-effective and robust methods that help developers improve software reliability and trustworthiness; study how modern AI methods — including large language models and agentic systems — can be used responsibly across testing, debugging, fault localization, and repair; and create high-quality datasets and benchmarks that help the community measure real progress in trustworthy software engineering. Our work spans both classical and quantum software systems.
      </p>
    </div>
  </div>
</section>

<section class="section section-alt" id="research">
  <div class="wrap split">
    <div class="split-label">
      <p class="eyebrow">Research</p>
      <h2>Research areas</h2>
      <p class="more"><a href="{{ '/project/' | relative_url }}">Read more about our research →</a></p>
    </div>

    <ol class="topics">
      <li>
        <div>
          <h3>Trustworthy AI for Software Engineering</h3>
          <div class="tags">
            <a class="tag" href="https://arxiv.org/pdf/2604.03447">arXiv ’26</a>
          </div>
        </div>
      </li>
      <li>
        <div>
          <h3>Automated Testing &amp; Test Oracles</h3>
          <div class="tags">
            <a class="tag" href="https://ieeexplore.ieee.org/abstract/document/10172745">ICSE ’23</a>
            <a class="tag" href="https://dl.acm.org/doi/abs/10.1145/3611643.3616265">FSE ’23</a>
            <a class="tag" href="https://dl.acm.org/doi/10.1145/3639478.3639791">ICSE-DS ’24</a>
            <a class="tag" href="https://ieeexplore.ieee.org/abstract/document/11029748">ICSE ’25</a>
            <a class="tag" href="https://dl.acm.org/doi/abs/10.1145/3729354">FSE ’25</a>
          </div>
        </div>
      </li>
      <li>
        <div>
          <h3>Automated Debugging &amp; Repair</h3>
          <div class="tags">
            <a class="tag" href="https://dl.acm.org/doi/10.5555/3737916.3739036">NeurIPS ’24</a>
            <a class="tag" href="https://dl.acm.org/doi/abs/10.1145/3660773">FSE ’24</a>
          </div>
        </div>
      </li>
      <li>
        <div>
          <h3>Tools, Datasets &amp; Benchmarks</h3>
          <div class="tags">
            <a class="tag" href="https://github.com/assert-lab/OE25-DEV">TOGBench · AIware ’26</a>
            <a class="tag" href="https://github.com/assert-lab/PITMuS">PITMuS · ASE ’26 Tools</a>
            <a class="tag" href="https://github.com/Geek-a-Byte/SWE-MIMIC-BENCH">SWE-MIMIC-BENCH</a>
            <a class="tag" href="https://github.com/assert-lab/CoCoMUT">CoCoMUT</a>
          </div>
        </div>
      </li>
      <li>
        <div>
          <h3>Quantum Software Testing</h3>
        </div>
      </li>
    </ol>
  </div>
</section>

<section class="section">
  <div class="wrap split">
    <div class="split-label">
      <p class="eyebrow">News</p>
      <h2>Recent news</h2>
      <p class="more"><a href="{{ '/news/' | relative_url }}">All news and updates →</a></p>
    </div>

    <ul class="news-list">
      {% for item in site.data.news limit: 4 %}
      <li class="news-item">
        <span class="news-date">{{ item.date }}</span>
        <span class="news-text">{{ item.text }}</span>
      </li>
      {% endfor %}
    </ul>
  </div>
</section>

<section class="section section-alt" id="join">
  <div class="wrap">
    <div class="join">
      <div>
        <p class="eyebrow">Join the lab</p>
        <h2>We are hiring PhD students.</h2>
        <div class="actions">
          <a class="btn btn-primary" href="mailto:{{ site.email }}">Get in touch</a>
        </div>
      </div>
      <div>
        <p>The AS²ERT Lab is looking for graduate students who are excited about software engineering research. If you are interested, we encourage you to take a look at our recent work and reach out with your thoughts on what current approaches miss and where the field could go next. Our lab culture values intellectual ownership, high standards, and deep technical engagement, along with open, principled discussion and follow-through. These values are closely aligned with these <a href="https://www.amazon.jobs/content/en/our-workplace/leadership-principles" target="_blank" rel="noopener">principles</a>.</p>
        <p><strong>Remote internships:</strong> We offer remote internship opportunities, particularly for international students. Please reach out via email if interested.</p>
      </div>
    </div>
  </div>
</section>

<section class="section">
  <div class="wrap split">
    <div class="split-label">
      <p class="eyebrow">Students</p>
      <h2>Undergraduate research</h2>
    </div>
    <div class="split-body">
      <p class="prose-lg">The AS²ERT Lab is deeply committed to mentoring motivated undergraduate students and helping them grow into confident, independent researchers in Software Engineering. UTD’s <strong>RIDE (Research, Inquiry, Design Experience)</strong> program provides an excellent foundation for introducing undergraduates to research in a structured and supportive environment. Through RIDE, students work on carefully scoped projects that encourage them to ask meaningful research questions, build and evaluate technical solutions, and communicate their findings at a level suitable for scholarly venues.</p>

      <ul class="ride">
        <li><span class="ride-code">RIDE 033</span>Trustworthy AI in Software Testing</li>
        <li><span class="ride-code">RIDE 041</span>Trustworthy AI in Software Engineering</li>
        <li><span class="ride-code">RIDE 045</span>Trustworthy AI in Quantum Software Engineering</li>
      </ul>
    </div>
  </div>
</section>
