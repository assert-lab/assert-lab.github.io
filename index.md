---
layout: single
author_profile: true
classes: wide
---

<style>
/* ===============================
   AS²ERT lab homepage redesign
   Content is preserved; this CSS only improves presentation.
   Scoped to this page to avoid affecting the rest of the site.
   =============================== */
:root {
  --as2ert-green: #154734;
  --as2ert-green-2: #23614a;
  --as2ert-orange: #E87500;
  --as2ert-ink: #172033;
  --as2ert-muted: #5f6b7a;
  --as2ert-line: rgba(21, 71, 52, 0.16);
  --as2ert-soft: #f7faf8;
  --as2ert-warm: #fff7ef;
  --as2ert-shadow: 0 16px 40px rgba(15, 23, 42, 0.08);
  --as2ert-shadow-soft: 0 10px 24px rgba(15, 23, 42, 0.06);
}

/* Page rhythm */
.page__content > .home-hero,
.page__content > .home-grid,
.page__content > .home-card {
  max-width: 1180px;
}

/* ===============================
   Hero
   =============================== */
.home-hero {
  position: relative;
  overflow: hidden;
  background:
    radial-gradient(circle at 92% 12%, rgba(232, 117, 0, 0.22), transparent 28%),
    radial-gradient(circle at 8% 90%, rgba(21, 71, 52, 0.12), transparent 34%),
    linear-gradient(135deg, #ffffff 0%, #fbfdfb 54%, rgba(21, 71, 52, 0.08) 100%);
  border: 1px solid var(--as2ert-line);
  border-radius: 26px;
  padding: clamp(24px, 4vw, 38px);
  box-shadow: var(--as2ert-shadow);
  margin-bottom: 22px;
  isolation: isolate;
}

.home-hero::before {
  content: "";
  position: absolute;
  inset: 14px;
  border: 1px solid rgba(21, 71, 52, 0.08);
  border-radius: 20px;
  pointer-events: none;
  z-index: -1;
}

.home-hero::after {
  content: "";
  position: absolute;
  right: -72px;
  bottom: -72px;
  width: 190px;
  height: 190px;
  border-radius: 999px;
  background: linear-gradient(135deg, rgba(232, 117, 0, 0.14), rgba(21, 71, 52, 0.08));
  filter: blur(4px);
  pointer-events: none;
  z-index: -1;
}

.home-hero h1 {
  margin: 0 0 6px 0;
  font-size: clamp(1.75rem, 3vw, 2.35rem);
  line-height: 1.12;
  letter-spacing: -0.035em;
  color: var(--as2ert-ink);
}

.home-hero .titleline {
  position: relative;
  margin: 0;
  max-width: 96ch;
  color: var(--as2ert-ink);
  line-height: 1.78;
  font-size: clamp(0.98rem, 1.25vw, 1.07rem);
}

.home-hero .titleline strong {
  color: var(--as2ert-green);
  font-weight: 800;
}

/* ===============================
   Main grid and cards
   =============================== */
.home-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 18px;
  align-items: stretch;
}

@media (min-width: 900px) {
  .home-grid {
    grid-template-columns: minmax(0, 0.95fr) minmax(0, 1.05fr);
  }
}

.home-card {
  position: relative;
  overflow: hidden;
  background: rgba(255, 255, 255, 0.96);
  border: 1px solid var(--as2ert-line);
  border-radius: 22px;
  padding: clamp(18px, 2.4vw, 24px);
  box-shadow: var(--as2ert-shadow-soft);
  transition: transform 180ms ease, box-shadow 180ms ease, border-color 180ms ease;
}

.home-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 18px 42px rgba(15, 23, 42, 0.10);
  border-color: rgba(21, 71, 52, 0.28);
}

.home-card::before {
  content: "";
  position: absolute;
  inset: 0 auto 0 0;
  width: 5px;
  background: linear-gradient(180deg, var(--as2ert-green), rgba(232, 117, 0, 0.55));
}

.home-card h2 {
  display: flex;
  align-items: center;
  gap: 10px;
  margin: 0 0 14px 0;
  font-size: clamp(1.18rem, 1.6vw, 1.42rem);
  line-height: 1.25;
  letter-spacing: -0.02em;
  color: var(--as2ert-green);
}

.home-card h2 i {
  display: inline-flex;
  width: 34px;
  height: 34px;
  align-items: center;
  justify-content: center;
  border-radius: 12px;
  background: rgba(21, 71, 52, 0.10);
  color: var(--as2ert-green);
  font-size: 0.95rem;
}

.home-card p {
  margin: 0 0 12px 0;
  color: var(--as2ert-ink);
  line-height: 1.76;
}

.home-card p:last-child {
  margin-bottom: 0;
}

.home-card a {
  color: var(--as2ert-orange);
  text-decoration: none;
  font-weight: 750;
}

.home-card a:hover {
  text-decoration: underline;
}

/* Research card highlight */
.home-grid .home-card:first-child {
  background:
    linear-gradient(135deg, rgba(21, 71, 52, 0.075), rgba(255, 255, 255, 0.90)),
    #ffffff;
}

/* ===============================
   Research list as polished feature rows
   =============================== */
.home-list {
  list-style: none;
  margin: 12px 0 0 0;
  padding: 0;
}

.home-list li {
  position: relative;
  display: block;
  margin: 10px 0;
  padding: 12px 12px 12px 46px;
  line-height: 1.55;
  border: 1px solid rgba(21, 71, 52, 0.12);
  border-radius: 16px;
  background: rgba(255, 255, 255, 0.82);
}

.home-list li > i:first-child {
  position: absolute;
  left: 13px;
  top: 13px;
  display: inline-flex;
  width: 26px;
  height: 26px;
  align-items: center;
  justify-content: center;
  border-radius: 10px;
  color: var(--as2ert-green);
  background: rgba(21, 71, 52, 0.10);
  font-size: 0.82rem;
}

.home-list strong {
  color: var(--as2ert-ink);
  font-weight: 850;
}

/* Paper badge links */
.paper-badge {
  display: inline-flex;
  align-items: center;
  margin: 4px 0 0 6px;
  padding: 3px 9px;
  font-size: 0.72rem;
  line-height: 1.2;
  font-weight: 800;
  border-radius: 999px;
  background: #ffffff;
  color: var(--as2ert-green) !important;
  text-decoration: none !important;
  border: 1px solid rgba(21, 71, 52, 0.18);
  vertical-align: middle;
  box-shadow: 0 2px 8px rgba(15, 23, 42, 0.04);
}

.paper-badge:hover {
  background: var(--as2ert-green);
  color: #ffffff !important;
  border-color: var(--as2ert-green);
  text-decoration: none !important;
}

/* ===============================
   Hiring CTA
   =============================== */
.cta {
  border-color: rgba(232, 117, 0, 0.28);
  background:
    radial-gradient(circle at 95% 8%, rgba(232, 117, 0, 0.20), transparent 30%),
    linear-gradient(135deg, #ffffff 0%, var(--as2ert-warm) 100%);
}

.cta::before {
  background: linear-gradient(180deg, var(--as2ert-orange), rgba(21, 71, 52, 0.55));
}

.cta .cta-title {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 12px;
  padding: 8px 12px;
  border-radius: 999px;
  background: rgba(232, 117, 0, 0.12);
  color: #8a3b00;
  font-weight: 950;
  letter-spacing: -0.01em;
}

/* ===============================
   Undergraduate / RIDE block
   =============================== */
.home-card[style*="margin-top:16px"] {
  margin-top: 18px !important;
  background:
    radial-gradient(circle at 100% 0%, rgba(21, 71, 52, 0.10), transparent 28%),
    #ffffff;
}

.ride-list {
  display: grid;
  grid-template-columns: 1fr;
  gap: 10px;
  margin: 16px 0 0 0;
  padding: 0;
  list-style: none;
  font-size: 0.95rem;
  line-height: 1.5;
}

@media (min-width: 760px) {
  .ride-list {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }
}

.ride-list li {
  position: relative;
  margin: 0;
  padding: 13px 14px 13px 16px;
  border: 1px solid rgba(21, 71, 52, 0.14);
  border-radius: 16px;
  background: var(--as2ert-soft);
  box-shadow: 0 6px 16px rgba(15, 23, 42, 0.04);
}

.ride-list li::before {
  content: "";
  position: absolute;
  left: 0;
  top: 14px;
  bottom: 14px;
  width: 4px;
  border-radius: 999px;
  background: var(--as2ert-orange);
}

.ride-list strong {
  color: var(--as2ert-green);
  font-weight: 850;
}

.note {
  font-size: 0.95rem;
  color: var(--as2ert-muted);
  margin-top: 10px;
  margin-bottom: 0;
}

@media (max-width: 640px) {
  .home-hero,
  .home-card {
    border-radius: 18px;
  }

  .home-list li {
    padding-right: 10px;
  }

  .paper-badge {
    margin-left: 2px;
    margin-right: 4px;
  }
}
</style>

<section class="home-hero">
  <p class="titleline">
    Howdy! Welcome to the <strong>AS²ERT </strong> (<strong>A</strong>I for <strong>S</strong>afe <strong>S</strong>oftware <strong>E</strong>ngineering and <strong>T</strong>esting) Lab at the University of Texas at Dallas (UTD). We develop automated techniques to improve the safety and reliability of software systems. Our research spans program analysis, testing, debugging, bug localization, and repair, with a focus on responsibly integrating modern AI methods, including large language models and agentic systems, into automated software engineering workflows.
</p>

  <p class="titleline" style="margin-top:10px;">
    AS²ERT lab is founded and led by <strong>Dr. Soneya Binta Hossain</strong>, Assistant Professor of Computer Science at UTD. She earned her Ph.D. and M.S in Computer Science from the University of Virginia, where her research explored AI-driven approaches to automated software testing. She earned her B.Sc. in Computer Science and Engineering from the Bangladesh University of Engineering and Technology (BUET). 
  </p>
</section>


<div class="home-grid">
  <section class="home-card">
    <h2><i class="fas fa-microscope"></i> Research Interests</h2>

    <ul class="home-list icon-list">
    <li>
  <i class="fas fa-clipboard-check"></i>
  <strong>Trustworthy AI for Software Engineering</strong>
  <a href="https://arxiv.org/pdf/2604.03447" class="paper-badge">arXiv’ 26</a>
</li>

      <li>
        <i class="fas fa-vial"></i>
        <strong>Automated Testing & Test Oracles</strong>
        <a href="https://ieeexplore.ieee.org/abstract/document/10172745" class="paper-badge">ICSE’23</a>
        <a href="https://dl.acm.org/doi/abs/10.1145/3611643.3616265" class="paper-badge">FSE’ 23</a>
        <a href="https://dl.acm.org/doi/10.1145/3639478.3639791" class="paper-badge">ICSE-DS’ 24</a>
        <a href="https://ieeexplore.ieee.org/abstract/document/11029748" class="paper-badge">ICSE’ 25</a>
        <a href="https://dl.acm.org/doi/abs/10.1145/3729354" class="paper-badge">FSE’ 25</a>
      </li>

      <li>
        <i class="fas fa-wrench"></i>
        <strong>Automated Debugging & Repair</strong>
         <a href="https://dl.acm.org/doi/10.5555/3737916.3739036" class="paper-badge">NIPS’ 24</a>
        <a href="https://dl.acm.org/doi/abs/10.1145/3660773" class="paper-badge">FSE ’24</a>
      </li>

      <li>
        <i class="fas fa-database"></i>
        <strong>Datasets & Benchmarks for Reliable SE</strong>
           <a href="https://github.com/assert-lab/OE25-DEV" class="paper-badge">TOGBench (AIware' 26)</a>
           <a href="https://github.com/Geek-a-Byte/SWE-MIMIC-BENCH" class="paper-badge">SWE-MIMIC-BENCH</a>
      </li>

      <li>
        <i class="fas fa-atom"></i>
        <strong>Quantum Software Testing</strong>
      </li>

    </ul>
</section>


  <aside class="home-card cta">
   <div class="cta-title">
    🚨 We are hiring PhD students!
  </div>
<p>
 The AS²ERT Lab is looking for graduate students who are excited about software engineering research. If you are interested, we encourage you to take a look at our recent work and reach out with your thoughts on what current approaches miss and where the field could go next. Our lab culture values intellectual ownership, high standards, and deep technical engagement, along with open, principled discussion and follow-through. These values are closely aligned with these
<a href="https://www.amazon.jobs/content/en/our-workplace/leadership-principles" target="_blank" rel="noopener">principles</a>.
</p>

<p style="margin-top:10px; margin-bottom:0;">
  <strong>Remote internships:</strong> We offer remote internship opportunities, particularly for international students. Please reach out via email if interested.
</p>

  </aside>
</div>

<section class="home-card" style="margin-top:16px;">
  <h2> Undergraduate Research</h2>

 <p>
  The AS²ERT Lab is deeply committed to mentoring motivated undergraduate students and helping them grow into confident, independent researchers in Software Engineering. UTD’s <strong>RIDE (Research, Inquiry, Design Experience)</strong> program provides an excellent foundation for introducing undergraduates to research in a structured and supportive environment. Through RIDE, students work on carefully scoped projects that encourage them to ask meaningful research questions, build and evaluate technical solutions, and communicate their findings at a level suitable for scholarly venues.
</p>

<ul class="ride-list">
  <li><strong>RIDE 033:</strong> Trustworthy AI in Software Testing</li>
  <li><strong>RIDE 041:</strong> Trustworthy AI in Software Engineering</li>
  <li><strong>RIDE 045:</strong> Trustworthy AI in Quantum Software Engineering</li>
</ul>
