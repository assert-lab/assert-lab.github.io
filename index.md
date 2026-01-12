---
layout: single
author_profile: true
classes: wide
---

<style>
/* ===============================
   Home page (scoped)
   =============================== */
.home-hero {
  background: linear-gradient(135deg, rgba(21,71,52,0.10), rgba(232,117,0,0.12));
  border: 1px solid rgba(0,0,0,0.06);
  border-radius: 18px;
  padding: 28px 28px;
  box-shadow: 0 12px 28px rgba(0,0,0,0.06);
  margin-bottom: 18px;
}

.home-hero h1 {
  margin: 0 0 6px 0;
  font-size: 2.0rem;
  line-height: 1.15;
}

.home-hero .titleline {
  margin: 0;
  opacity: 0.92;
  line-height: 1.6;
  max-width: 90ch;
}

.home-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 16px;
}

@media (min-width: 860px) {
  /* Research (first card) smaller, Prospective PhD (second card) larger */
  .home-grid {
    grid-template-columns: 0.85fr 1.15fr;
  }
}

.home-card {
  background: #ffffff;
  border: 1px solid rgba(0,0,0,0.07);
  border-radius: 16px;
  padding: 18px 18px;
  box-shadow: 0 10px 22px rgba(0,0,0,0.05);
}

.home-card h2 {
  margin-top: 0;
  margin-bottom: 10px;
  font-size: 1.35rem;
}

.home-card p {
  margin: 0 0 10px 0;
  line-height: 1.7;
}

.cta {
  border-left: 5px solid #E87500;
  background: rgba(232,117,0,0.10);
}

.cta .cta-title {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  font-weight: 950;
  margin-bottom: 8px;
}

.home-list {
  margin: 10px 0 0 0;
  padding-left: 18px;
}

.home-list li {
  margin: 8px 0;
  line-height: 1.6;
}

.note {
  font-size: 0.95rem;
  opacity: 0.92;
  margin-top: 10px;
  margin-bottom: 0;
}
  /* Research interest card highlight */
.home-grid .home-card:first-child {
  background:
    linear-gradient(
      135deg,
      rgba(21, 71, 52, 0.08),   /* UTD green */
      rgba(21, 71, 52, 0.03)
    ),
    #ffffff;
  border: 1px solid rgba(21, 71, 52, 0.25);
}

/* Optional: subtle accent on the title */
.home-grid .home-card:first-child h2 {
  color: #154734; /* UTD Green */
}
/* Paper badge links */
.paper-badge {
  display: inline-block;
  margin-left: 6px;
  padding: 2px 8px;
  font-size: 0.7rem;
  font-weight: 600;
  border-radius: 999px;
  background: #f3f4f6;
  color: #154734; /* UTD green */
  text-decoration: none;
  border: 1px solid #d1d5db;
  vertical-align: middle;
}

.paper-badge:hover {
  background: #154734;
  color: #ffffff;
  border-color: #154734;
}

</style>

<section class="home-hero">
  <h1 style="color:#154734;">Howdy!</h1>

  <p class="titleline">
    Welcome to the <strong>AS²ERT Lab</strong> (<strong>A</strong>I for <strong>S</strong>afe <strong>S</strong>oftware <strong>E</strong>ngineering and <strong>T</strong>esting) at the University of Texas at Dallas (UTD). Because software runs much of the world and must be worthy of users’ trust, our broader goal is to develop automated techniques that help build safe and reliable software systems. Our group primarily focuses on automated testing, debugging, and repair, with particular attention to requirements-aware test automation. We are especially interested in how modern AI methods, including large language models and agentic AI, can be used responsibly to improve software quality in ways that are both effective and practical.
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
        <i class="fas fa-vial"></i>
        <strong>Automated testing and test oracles</strong>
        <a href="https://ieeexplore.ieee.org/abstract/document/10172745" class="paper-badge">ICSE’23</a>
        <a href="https://dl.acm.org/doi/abs/10.1145/3611643.3616265" class="paper-badge">FSE’ 23</a>
        <a href="https://dl.acm.org/doi/10.1145/3639478.3639791" class="paper-badge">ICSE-DS’ 24</a>
        <a href="https://ieeexplore.ieee.org/abstract/document/11029748" class="paper-badge">ICSE’ 25</a>
        <a href="https://dl.acm.org/doi/abs/10.1145/3729354" class="paper-badge">FSE’ 25</a>
      </li>

      <li>
        <i class="fas fa-clipboard-check"></i>
        <strong>Requirements-aware software testing</strong>
         <a href="https://dl.acm.org/doi/abs/10.1145/3729354" class="paper-badge">FSE’ 25</a>
      </li>

      <li>
        <i class="fas fa-bug"></i>
        <strong>Automated bug localization and debugging</strong>
        <a href="https://dl.acm.org/doi/10.5555/3737916.3739036" class="paper-badge">NIPS’ 24</a>
      </li>

      <li>
        <i class="fas fa-wrench"></i>
        <strong>AI-assisted program repair</strong>
        <a href="https://dl.acm.org/doi/abs/10.1145/3660773" class="paper-badge">FSE ’24</a>
      </li>

      <li>
        <i class="fas fa-database"></i>
        <strong>Data-centric foundations for reliable testing</strong>
      </li>

      <li>
        <i class="fas fa-atom"></i>
        <strong>Automated testing for quantum software</strong>
      </li>

    </ul>
</section>


  <aside class="home-card cta">
   <div class="cta-title">
    🚨 We are hiring PhD students!
  </div>

    <p>
   I enjoy working with students who are highly passionate about advancing the field of Software Engineering. Please read my recent publications and reach out to share your thoughts on (1) limitations you see in existing work and (2) potential ideas for addressing them.
Curious whether you might be a good fit for the AS²ERT Lab? I encourage you to review the <a href="https://www.amazon.jobs/content/en/our-workplace/leadership-principles" target="_blank" rel="noopener">
    Amazon Leadership Principles
  </a>. Principles such as ownership, high standards, diving deep, and thoughtful disagreement with commitment resonate strongly with how I approach research and collaboration.
    </p>

    <p style="margin-top:10px; margin-bottom:0;">
      <strong>Remote internships:</strong> We welcome applications from international students interested in remote internship opportunities. Please reach out via email.
    </p>
  </aside>
</div>

<section class="home-card" style="margin-top:16px;">
  <h2> Undergraduate Research</h2>

  <p>
   It is my great pleasure to work with motivated undergraduate students and to help prepare the next generation of researchers in Software Engineering. UTD’s <strong>RIDE (Research, Inquiry, Design Experience)</strong> program is an excellent initiative that supports undergraduate research and provides students with early exposure to the research process. Through RIDE, projects are carefully structured to help students identify well-scoped research problems, develop and rigorously evaluate technical solutions, and communicate their findings at a level appropriate for publication.
  </p>

  <ul class="home-list">
    <li><strong>Project 1:</strong> Resilient LLMs for reasoning about buggy code.</li>
    <li><strong>Project 2:</strong> Quantum software testing benchmarks and bug taxonomies.</li>
    <li><strong>Project 3:</strong> High-quality automated documentation generation to support testing.</li>
  </ul>

  <p class="note">
    UTD undergraduates: please email your resume and transcript (unofficial is fine), along with a
    brief explanation of which project you are interested in and why.
  </p>
</section>
