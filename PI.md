---
layout: single
permalink: /PI/
classes: wide
title: ""
author_profile: true
---

<style>
  /* --- PI Grid + Cards --- */
  .pi-grid {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    gap: 18px;
    font-size: .8rem;
    align-items: start;
  }
  @media (max-width: 1024px) {
    .pi-grid { grid-template-columns: repeat(6, 1fr); }
  }
  @media (max-width: 640px) {
    .pi-grid { grid-template-columns: repeat(2, 1fr); }
  }
  .pi-card {
    grid-column: span 6; /* default: 2-up */
    background: #fff;
    border: 2px solid #ff6600;
    border-radius: 14px;
    padding: 18px 18px 14px;
    font-size: .8rem;
    box-shadow: 0 6px 18px rgba(0,0,0,0.06);
  }
  .pi-card h3 {
    margin: 0 0 10px 0;
    font-size: .8rem;
    line-height: 1.3;
  }
  .pi-card .pill {
    display: inline-block;
    background: #2E6F40;
    border: 1px solid #ff6600;
    color: #333;
    padding: 2px 8px;
    border-radius: 999px;
    font-size: 0.8rem;
    margin-left: 8px;
    vertical-align: middle;
  }
  .pi-accent { color: #ff6600; font-weight: 700; }
  .pi-card a { color: #ff6600; text-decoration: none; }
  .pi-card a:hover { text-decoration: underline; }

  /* Featured (full width) and tall/scrollable variants */
  .span-12 { grid-column: span 12; }
  .span-8  { grid-column: span 8; }
  .span-4  { grid-column: span 4; }
  .pi-scroll {
    max-height: 420px;
    overflow: auto;
    padding-right: 6px;
  }

  /* Subtle list spacing */
  .pi-card ul { margin: 8px 0 0 18px; }
  .pi-card li { margin: 6px 0; }
</style>

<div class="pi-grid">

  <!-- ABOUT / HERO -->
  <section class="pi-card span-12">
    <h3><span class="pill">UT Dallas • Software Engineering</span></h3>
<p>
  I earned my <strong>Ph.D. in Computer Science</strong> from the <strong>University of Virginia</strong> in Summer 2025, where I was advised by
  <a href="https://matthewbdwyer.github.io/">Dr. Matthew Dwyer</a>.
  Broadly, my research area is <strong>AI for Software Engineering</strong>, with a focus on <em>requirements, testing, debugging, and repair</em> for both classical and quantum software.
  My long-term vision is to advance the development of high-quality, reliable software through <em>cost-effective automation</em> powered by <strong>AI/ML, large language models (LLMs),</strong> and <strong>agentic AI</strong>.
</p>

<p>
  During my Ph.D., I collaborated with <strong>Lockheed Martin</strong> and multiple teams at <strong>AWS</strong> (CodeGuru, CodeCatalyst, and AWS AI Labs),
  and my work has been published in premier venues including <strong>ICSE, FSE, and NeurIPS</strong>.
</p>

  </section>

  <!-- EDUCATION -->
  <section class="pi-card span-12">
    <h3><span class="pill">Education</span</h3>
    <ul>
      <li><strong>Ph.D., Computer Science</strong>, University of Virginia<br>
        Advisor: Matthew Dwyer • Committee: Sebastian Elbaum, Yangfeng Ji, Matthew Bolton, Antonio Filieri<br>
        Thesis: <em>Assessing and Improving Critical Properties of Test Oracles for Effective Software Bug Detection.</em>
      </li>
      <li><strong>MCS, Computer Science</strong>, University of Virginia<br>
        Project: <em>TOGLL: Correct and Strong Test Oracle Generation with LLMs.</em>
      </li>
      <li><strong>B.Sc., CSE</strong>, BUET<br>
        Thesis: <em>Balanced Coverage in Fault-Tolerant Broadcasting for Wireless Multi-hop Networks.</em>
      </li>
    </ul>
  </section>

 

  <!-- RESEARCH AWARDS -->
  <section class="pi-card span-12">
    <h3><span class="pill">Research Awards</span</h3>
    <ul>
      <li><strong>Copenhaver Charitable Trust Bicentennial Fellow</strong>, UVA (2024–2025), $12,000.</li>
      <li><strong>Finalist</strong>, UVA Research Computing Exhibition 2024 (Rivanna HPC).</li>
      <li><strong>John A. Stankovic Outstanding Graduate Research Award</strong> (2022–2023), CS @ UVA
        <a href="https://engineering.virginia.edu/department/computer-science/blogs/cs-department-end-year-award-recipients-2022-2023">link</a>
      </li>
      <li><strong>Student Choice Best Research Award</strong>, 2023 CS Research Symposium
        <a href="https://engineering.virginia.edu/department/computer-science/blogs/2023-cs-research-symposium-highlights">link</a>
      </li>
      <li><strong>Best Research Poster</strong>, 2021 CS Research Symposium
        <a href="https://uvaeng.prod.acquia-sites.com/events/2021-fall-cs-research-symposium">link</a>
      </li>
      <li><strong>PhD Fellowship</strong>, CS @ UVA (2019)</li>
      <li><strong>Outstanding Undergraduate Thesis</strong>, CSE @ BUET (2016)</li>
    </ul>
  </section>

  <!-- SERVICE AWARD -->
  <section class="pi-card span-6">
    <h3>Service Award</h3>
    <ul>
      <li><strong>Outstanding Service Award</strong>, CS @ UVA (2022)
        <a href="https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards">link</a>
        <br>
        <span>
          <em>Leadership Chair</em>, CSGSG for two years; organized leadership/social events; bridged students and department; organized the CS Research Symposium in 2020 & 2021.
        </span>
      </li>
    </ul>
  </section>

  <!-- TRAVEL GRANTS -->
  <section class="pi-card span-6">
    <h3>Travel Grants</h3>
    <ul>
      <li>ACM SIGSOFT travel grant — FSE’25, Trondheim, Norway.</li>
      <li>CRA travel grants — Grad Cohort (2023 San Francisco, 2020 New Orleans).</li>
      <li>SWE24 — Chicago, IL (Oct 23–26, 2024).</li>
      <li>Grace Hopper (GHCI) — Bangalore, India (2015).</li>
    </ul>
  </section>

  <!-- UNDERGRAD ACADEMIC AWARDS -->
  <section class="pi-card span-6">
    <h3>Undergraduate Academic Awards</h3>
    <ul>
      <li><strong>Top Ten Database Project</strong>, CSE @ BUET (2014)</li>
      <li><strong>Dean’s List (Level-2)</strong>, CSE @ BUET (2013–2014)</li>
      <li><strong>University Merit Scholarship</strong>, CSE @ BUET (2013–2014)</li>
    </ul>
  </section>

  <!-- SERVICE -->
  <section class="pi-card span-6">
    <h3>Service</h3>
    <ul>
      <li><strong>Program Committee</strong>: ACM TOSEM; IEEE ICST 2024.</li>
      <li><strong>Student Volunteer</strong>: SWE WE24 (Chicago, 2024); ESEC/FSE 2023 (San Francisco).</li>
      <li><strong>Leadership Chair</strong>: CSGSG, UVA (Jan’20–Dec’22).</li>
      <li><strong>Social Chair</strong>: ABS, UVA (Fall’21–Summer’22).</li>
    </ul>
  </section>

  <!-- TEACHING & MENTORING -->
  <section class="pi-card span-6">
    <h3>Teaching & Mentoring</h3>
    <ul>
      <li><strong>Graduate TA</strong>: CS 4620 (Undergrad Compilers), CS 6620 (Grad Compilers), UVA.</li>
      <li><strong>Mentor (UVA)</strong> — research & grad-school prep; mentees include:
        Raygan Taylor (DU), Javan Mendoza (UMBC), Nicki Choquette (UVA), Kasra Lekan (UVA), Ashley Hart (UCF), Srikar Chittari (UVA), Eric Weng (UVA).
      </li>
      <li><strong>BWCSE Mentor</strong> — mentoring BUET 3rd/4th years on research and applications.</li>
    </ul>
  </section>

  <!-- NEWS (SCROLLABLE) -->
  <section class="pi-card span-12 pi-scroll">
    <h3>News</h3>
    <ul>
      <li><strong>Aug 1, 2025</strong>: Joined CS@UTD as a Tenure-track Assistant Professor.</li>
      <li><strong>Jul 25, 2025</strong>: Relocated to Dallas, TX from beautiful Virginia.</li>
      <li><strong>Jun 25, 2025</strong>: Attended FSE’25 (Trondheim); presented <a href="https://dl.acm.org/doi/abs/10.1145/3729354">Doc2OracLL</a>.</li>
      <li><strong>Apr 25, 2025</strong>: Attended ICSE’25 (Ottawa); presented <a href="https://ieeexplore.ieee.org/document/11029748">TOGLL</a>.</li>
      <li><strong>Apr 25, 2025</strong>: Successfully defended PhD (Dr. Soneya Binta Hossain!).</li>
      <li><strong>Apr 2025</strong>: Paper accepted at FSE’25: <a href="https://dl.acm.org/doi/abs/10.1145/3729354">Doc2Oracle</a>.</li>
      <li><strong>Nov 2024</strong>: Paper accepted at ICSE’25: <a href="https://ieeexplore.ieee.org/document/11029748">TOGLL</a>.</li>
      <li><strong>Sep 2024</strong>: Travel grant to SWE24 (Oct 23–26, Chicago).</li>
      <li><strong>Sep 2024</strong>: Received UVA’s prestigious Endowed Fellowship ($12,000).</li>
      <li><strong>May 2024</strong>: Earned MCS (UVA) with CGPA 4.0/4.0. [gallery]</li>
      <li><strong>May 2024</strong>: Defended PhD proposal — *Assessing and Improving Critical Properties of Test Oracles…* [gallery]</li>
      <li><strong>Apr 2024</strong>: ICSE’24 (Lisbon) Doctoral Symposium [gallery]</li>
      <li><strong>Apr 2024</strong>: Finalist — UVA Research Computing Exhibition 2024.</li>
      <li><strong>Apr 2024</strong>: FSE’24: <a href="https://dl.acm.org/doi/abs/10.1145/3660773">LLMs for Bug Localization & Repair</a>.</li>
      <li><strong>Dec 2023</strong>: ICSE’24 Doctoral Symposium paper accepted.</li>
      <li><strong>Dec 2023</strong>: Presented FSE’23 paper [gallery]</li>
      <li><strong>Oct 2023</strong>: Student Choice Research Award (UVA CS Symposium 2023).</li>
      <li><strong>Jul 2023</strong>: FSE’23 research paper accepted.</li>
      <li><strong>Jun 2023</strong>: Summer internship at AWS CodeCatalyst (Santa Clara).</li>
      <li><strong>May 2023</strong>: ICSE’23 (Melbourne) presentation [gallery]</li>
      <li><strong>May 2023</strong>: John A. Stankovic Outstanding Graduate Research Award [gallery]</li>
      <li><strong>Apr 2023</strong>: CRA Grad Cohort (San Francisco) [gallery]</li>
      <li><strong>Feb 2023</strong>: ICSE’23 Artifact Evaluation Track — <a href="https://github.com/soneyahossain/hcc-gap-recommender">HCC recommender</a>.</li>
      <li><strong>Dec 2022</strong>: ICSE’23 tech track — <a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10172745">HCC paper</a>.</li>
      <li><strong>May 2022</strong>: AWS CodeGuru internship (Seattle).</li>
      <li><strong>May 2022</strong>: Outstanding Graduate Service Award (UVA) [gallery]</li>
      <li><strong>Apr 2022</strong>: ICSE’22 (Pittsburgh).</li>
      <li><strong>Dec 2021</strong>: Outstanding Research Poster (UVA CS Symposium).</li>
      <li><strong>Dec 2021</strong>: Organized CS Dept Research Symposium (news, tweet).</li>
      <li><strong>Sep 2021</strong>: Passed Ph.D. Qualifying Exam.</li>
      <li><strong>Apr 2021</strong>: CRA-W Grad Cohort 2021 (virtual).</li>
      <li><strong>Feb 2021</strong>: TA for Graduate Compilers (CS 6620), Prof. Dwyer.</li>
      <li><strong>Aug 2019</strong>: Started Ph.D. in CS @ UVA.</li>
    </ul>
  </section>

</div>
