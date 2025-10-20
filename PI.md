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
    border: 2px solid #2E6F40;
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
    background: #ff6600;
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

<div style="background:#fff4e6; border:2px solid #ff6600; border-radius:10px; padding:10px 15px; margin-bottom:20px; font-size:0.95em;">
  <strong>Archived Page:</strong> A look into my Ph.D. years and journey before becoming a professor.
  For current updates, see the
  <a href="/news/" style="color:#ff6600; font-weight:600;">Lab News</a> and
  <a href="/publications/" style="color:#ff6600; font-weight:600;">Publications</a> pages.
</div>

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
    <h3><span class="pill">Education</span></h3>
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
    <h3><span class="pill">Research Awards</span></h3>
    <ul>
      <li><strong>Copenhaver Charitable Trust Bicentennial Fellow</strong>, UVA (2024–2025), $12,000.</li>
      <li><strong>Finalist</strong>, UVA Research Computing Exhibition 2024 (Rivanna HPC), UVA.</li>
      <li><strong>John A. Stankovic Outstanding Graduate Research Award</strong> (2022–2023), CS, UVA
        <a href="https://engineering.virginia.edu/department/computer-science/blogs/cs-department-end-year-award-recipients-2022-2023">link</a>
      </li>
      <li><strong>Student Choice Best Research Award</strong>, 2023 CS Research Symposium, UVA
        <a href="https://engineering.virginia.edu/department/computer-science/blogs/2023-cs-research-symposium-highlights">link</a>
      </li>
      <li><strong>Best Research Poster</strong>, 2021 CS Research Symposium, UVA
        <a href="https://uvaeng.prod.acquia-sites.com/events/2021-fall-cs-research-symposium">link</a>
      </li>
      <li><strong>PhD Fellowship</strong>, CS, UVA (2019)</li>
      <li><strong>Outstanding Undergraduate Thesis</strong>, CSE, BUET (2016)</li>
    </ul>
  </section>

  <!-- SERVICE AWARD -->
  <section class="pi-card span-12">
    <h3><span class="pill">Service Award</span></h3>
    <ul>
      <li><strong>Outstanding Graduate Service Award</strong>, CS @ UVA (2022)
        <a href="https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards">link</a>
        <br>
        <span>
          <em>Leadership Chair</em>, the Computer Science Graduate Student Group (CSGSG) for two years; organized leadership/social events; bridged students and department; organized the CS Research Symposium in 2020 & 2021.
        </span>
      </li>
    </ul>
  </section>

  <!-- TRAVEL GRANTS -->
   <section class="pi-card span-12">
    <h3><span class="pill">Travel Grants</span></h3>
    <ul>
      <li>ACM SIGSOFT travel grant — FSE’25, Trondheim, Norway.</li>
      <li>CRA travel grants — Grad Cohort (2023 San Francisco, 2020 New Orleans).</li>
      <li>The Society of Women Engineers (SWE)'24 — Chicago, IL (Oct 23–26, 2024).</li>
      <li>Grace Hopper Celebration (GHCI) — Bangalore, India (2015).</li> 
    </ul>
  </section>

  <!-- UNDERGRAD ACADEMIC AWARDS -->
  <section class="pi-card span-12">
    <h3><span class="pill">Undergraduate Academic Awards</span></h3>
    <ul>
      <li><strong>Top Ten Database Project</strong>, CSE, BUET (2014)</li>
      <li><strong>Dean’s List (Level-2)</strong>, CSE, BUET (2013–2014)</li>
      <li><strong>University Merit Scholarship</strong>, CSE, BUET (2013–2014)</li>
    </ul>
  </section>


  <!-- NEWS (SCROLLABLE) -->
  <section class="pi-card span-12 pi-scroll">
    <h3><span class="pill">News</span></h3>
    <ul>
     
### News
- **August 1, 2025**: Joined CS@UTD as a Tenure-track Assistant Professor.  
- **July 25, 2025**: Relocated to Dallas, TX from beautiful Virginia.  
- **June 25, 2025**: Attended FSE 2025 in Trondheim, Norway, and presented my paper [Doc2OracLL](https://dl.acm.org/doi/abs/10.1145/3729354).  
- **April 25, 2025**: Attended ICSE 2025 in Ottawa, Canada, and presented my paper [TOGLL](https://ieeexplore.ieee.org/document/11029748).  
- **April 25, 2025**: I successfully defended my PhD and officially became Dr. Soneya Binta Hossain!  
- **April 2025**: My paper [Doc2Oracle: Investigating the Impact of Javadoc Comments on Test Oracle Generation](https://dl.acm.org/doi/abs/10.1145/3729354) is accepted at FSE'25 Research Track.
- **Nov 2024**: My paper [TOGLL: Correct and Strong Test Oracle Generation with LLMs](https://ieeexplore.ieee.org/document/11029748) is accepted at ICSE'25 Research Track.
- **Sep 2024**: Received travel grant to attend the SWE24 — the world's largest conference for women in engineering and technology—from October 23–26 in Chicago, IL.
- **Sep 2024**: Received UVA's most prestigious Endowed Fellowship! This fellowship is awarded to outstanding doctoral students with an award of $12,000.
- **May 2024**: Received Master of Computer Science (MCS) from UVA with a CGPA of 4.0/4.0! [\[gallery\]](graduation.md)
- **May 2024**:  Defended my PhD dissertation proposal, titled *Assessing and Improving Critical Properties of Test Oracles for
Effective Software Bug Detection* [\[gallery\]](proposal.md)
- **April 2024**: Attended ICSE'24 in beautiful Lisbon, Portugal, and presented my paper at the doctoral symposium [\[gallery\]](icse-24.md)
- **April 2024**: Honored to be selected as one of the five finalists at UVA Research Computing Exhibition 2024!
- **April 2024**: My paper [A Deep Dive into Large Language Models for Automated Bug Localization and Repair](https://dl.acm.org/doi/abs/10.1145/3660773) is accepted at FSE'24 Research Track.
- **December 2023**: My paper [Ensuring Critical Properties of Test Oracles for Effective Bug Detection](https://dl.acm.org/doi/10.1145/3639478.3639791) is accepted at the ICSE'24 Doctoral Symposium.
- **December 2023**: Presented our paper [Neural-Based Test Oracle Generation: A Large-Scale Evaluation
and Lessons Learned](https://dl.acm.org/doi/pdf/10.1145/3611643.3616265) at FSE'23 (Dec 3-9) in San Francisco, CA [\[gallery\]](FSE-23.md)
- **October 2023**: Honored to receive [Student Choice Research Award](https://engineering.virginia.edu/department/computer-science/blogs/2023-cs-research-symposium-highlights) at CS Department Research Symposium 2023.
- **July 2023**: Our paper [Neural-Based Test Oracle Generation: A Large-scale Evaluation and Lessons Learned](https://dl.acm.org/doi/abs/10.1145/3611643.3616265) is accepted at the FSE'23 research track.
- **June 2023**: Started summer internship at AWS CodeCatalyst team in Santa Clara, CA.
- **May 2023**: Presented our [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10172745) at ICSE'23 in Melbourne, Australia [\[gallery\]](ICSE-23.md)
- **May 2023**: Received the [John A. Stankovic Outstanding Graduate Research Award](https://engineering.virginia.edu/department/computer-science/blogs/cs-department-end-year-award-recipients-2022-2023) [\[gallery\]](award-23.md)
- **April 2023**: Attended CRA Grad Cohort in San Francisco, CA [\[gallery\]](CRA-SFO.md)
- **February 2023**: Our research [artifact](https://github.com/soneyahossain/hcc-gap-recommender) is accepted at the [ICSE Artifact Evaluation Track](https://conf.researchr.org/details/icse-2023/icse-2023-artifact-evaluation/5/Artifact-Measuring-and-Mitigating-Gaps-in-Structural-Testing).
- **December 2022**: Our paper on [Measuring and Mitigating Gaps in Structural Testing](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10172745) is accepted at the ICSE'23 technical track.
- **May 2022**: Started summer internship at AWS Code Guru team in Seattle, WA.
- **May 2022**: Received [Outstanding Graduate Service Award](https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards) [\[gallery\]](service-award.md)
- **April 2022**: Attended ICSE'22 in Pittsburgh.
- **December 2021**: Received [Outstanding Research Poster Award](https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards) at CS Research Symposium.
- **December 2021**: Organized [CS Department Research Symposium](https://uvaeng.prod.acquia-sites.com/events/2021-fall-cs-research-symposium), [News](https://engineering.virginia.edu/labs-groups/link-lab/blogs/computer-science-graduate-student-group-research-symposium), [Tweet](https://twitter.com/CS_UVA/status/1471529342912155650?s=20&t=YbVecueDVPOLsdDaw0sBfQ).
- **September 2021**: Passed the Ph.D. Qualifying Exam with flying colors!
- **April 2021**: Attended the CRA-W Grad Cohort Workshop 2021 (virtual due to COVID-19).
- **February 2021**: Started working as a TA for graduate compilers (CS 6620) by Prof. Matt Dwyer.
- **August 2019**: Started Ph.D. in CS at the University of Virginia.

    </ul>
  </section>

</div>
