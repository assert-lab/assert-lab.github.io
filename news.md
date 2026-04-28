---
layout: single
permalink: /news/
classes: wide
title: "News & Updates"
author_profile: true
---

<style>
/* ===============================
   News page (scoped, matching index.md visual theme)
   =============================== */
.news-page {
  --utd-green: #154734;
  --utd-orange: #E87500;
  --news-ink: #1f2937;
  --news-line: rgba(0,0,0,0.07);
  --news-shadow: 0 10px 22px rgba(0,0,0,0.05);
  color: var(--news-ink);
  font: inherit;
  font-size: 0.98rem;
  line-height: 1.65;
}

.news-page a {
  color: var(--utd-orange);
  text-decoration: none;
  font-weight: 700;
}

.news-page a:hover {
  text-decoration: underline;
}

.news-page .home-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 16px;
}

.news-page .home-card {
  background: #ffffff;
  border: 1px solid var(--news-line);
  border-radius: 16px;
  padding: 18px 18px;
  box-shadow: var(--news-shadow);
  position: relative;
  overflow: hidden;
}

.news-page .home-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  width: 5px;
  background: linear-gradient(180deg, var(--utd-green), rgba(232,117,0,0.72));
}

.news-page .home-card h2 {
  margin-top: 0;
  margin-bottom: 12px;
  padding-left: 10px;
  font-size: 1.35rem;
  color: var(--utd-green);
}

.news-page .home-card.highlight {
  background:
    linear-gradient(135deg, rgba(21, 71, 52, 0.08), rgba(21, 71, 52, 0.03)),
    #ffffff;
  border: 1px solid rgba(21, 71, 52, 0.25);
}

.news-list {
  list-style: none;
  margin: 0;
  padding: 0 0 0 10px;
}

.news-list li {
  display: grid;
  grid-template-columns: 128px 1fr;
  gap: 12px;
  padding: 12px 0;
  border-top: 1px solid rgba(0,0,0,0.07);
  line-height: 1.65;
}

.news-list li:first-child {
  border-top: 0;
  padding-top: 0;
}

.news-date {
  color: var(--utd-orange);
  font-weight: 850;
  white-space: nowrap;
}

.news-text strong {
  color: var(--utd-green);
}

@media (max-width: 700px) {
  .news-list li {
    grid-template-columns: 1fr;
    gap: 2px;
  }
  .news-date {
    white-space: normal;
  }
}
</style>

<div class="news-page">
<div class="home-grid">

  <section class="home-card highlight" id="2026">
    <h2>2026</h2>
    <ul class="news-list">
      <li>
        <span class="news-date">April 2026</span>
        <span class="news-text">Our dataset and benchmark paper, “TOGBench: A Developer-Written Multi-Variant Dataset and Benchmark Suite for Test Oracle Generation,” has been accepted to the 3rd ACM International Conference on AI-Powered Software (AIware 2026)!</span>
      </li>
      <li>
        <span class="news-date">April 2026</span>
        <span class="news-text">Our research paper, “Measuring LLM Trust Allocation Across Conflicting Software Artifacts,” is now available on <a href="https://arxiv.org/abs/2604.03447">arXiv</a>.</span>
      </li>
      <li>
        <span class="news-date">April 2026</span>
        <span class="news-text">Our paper, “From Threads to Trajectories: A Multi-LLM Pipeline for Community Knowledge Extraction from GitHub Issue Discussions,” is now available on arXiv.</span>
      </li>
      <li>
        <span class="news-date">April 2026</span>
        <span class="news-text">Dr. Hossain joined the Program Committee (PC) of the ASE 2026 Tools and Datasets track!</span>
      </li>
      <li>
        <span class="news-date">April 2026</span>
        <span class="news-text">Dr. Hossain joined the Program Committee (PC) of the 2027 edition of FSE, the ACM International Conference on the Foundations of Software Engineering!</span>
      </li>
      <li>
        <span class="news-date">Feb 2026</span>
        <span class="news-text">Noshin Ulfat (incoming PhD student at the AS²ERT Lab) received UTD’s prestigious <strong>Presidential Fellowship</strong>, totaling $37,000.</span>
      </li>
      <li>
        <span class="news-date">Feb 2026</span>
        <span class="news-text">Dr. Hossain joined the Program Committee of FSE'26 Ideas, Visions and Reflections (IVR) track!</span>
      </li>
      <li>
        <span class="news-date">January 2026</span>
        <span class="news-text">Dr. Hossain joined the Program Committee of 3rd ACM International Conference on AI-powered Software (AIware 2026), co-located with FSE'26!</span>
      </li>
      <li>
        <span class="news-date">January 2026</span>
        <span class="news-text">Tasfia joined the AS²ERT Lab as a PhD student. Welcome to the lab!</span>
      </li>
      <li>
        <span class="news-date">January 2026</span>
        <span class="news-text">Dr. Hossain joined the Program Committee of ICST 2026.</span>
      </li>
      <li>
        <span class="news-date">2026</span>
        <span class="news-text">Dr. Hossain continued serving as a Program Committee member for ACM TOSEM.</span>
      </li>
    </ul>
  </section>

  <section class="home-card" id="2025">
    <h2>2025</h2>
    <ul class="news-list">
      <li>
        <span class="news-date">Dec 2025</span>
        <span class="news-text">Dr. Hossain received two <strong>URAP</strong> (Undergraduate Research Apprenticeship Program) Summer 2026 awards, supporting two undergraduate researchers with summer stipends to conduct research in Software Engineering and Quantum Computing!</span>
      </li>
      <li>
        <span class="news-date">Dec 2025</span>
        <span class="news-text">Dr. Hossain received the <strong>Grace Hopper Spirit Award</strong> from the Department of Computer Science at UT Dallas, recognizing her service and contributions to the department.</span>
      </li>
      <li>
        <span class="news-date">Aug 2025</span>
        <span class="news-text">Dr. Hossain began teaching <strong>CS/CE/SE 3354: Software Engineering</strong>; she is also serving as the course coordinator for this course.</span>
      </li>
      <li>
        <span class="news-date">Aug 2025</span>
        <span class="news-text">Dr. Hossain joined the Department of Computer Science at The University of Texas at Dallas as an Assistant Professor and founded the <strong>AS²ERT Lab (AI for Safe Software Engineering and Testing)</strong>.</span>
      </li>
    </ul>
  </section>

</div>
</div>
