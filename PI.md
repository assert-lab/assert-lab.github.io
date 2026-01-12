---
layout: single
permalink: /PI/
classes: wide
title: ""
author_profile: true
---

<style>
  /* --- Theme tokens (easy to tweak) --- */
  :root{
    --pi-green:#2E6F40;
    --pi-orange:#ff6600;
    --pi-text:#1f2937;
    --pi-muted:#6b7280;
    --pi-border: rgba(46,111,64,.20);
    --pi-shadow: 0 10px 28px rgba(0,0,0,.06);
  }

  /* --- Grid --- */
  .pi-grid{
    display:grid;
    grid-template-columns: repeat(12, 1fr);
    gap:18px;
    align-items:start;

    font: inherit;
    font-size: 0.98rem;
    line-height: 1.65;
    color: var(--pi-text);
  }
  @media (max-width: 1024px){ .pi-grid{ grid-template-columns: repeat(6, 1fr); } }
  @media (max-width: 640px){ .pi-grid{ grid-template-columns: repeat(2, 1fr); } }

  /* --- Cards (not boxy, but still structured) --- */
  .pi-card{
    grid-column: span 6;
    background:#fff;
    border:1px solid var(--pi-border);
    border-radius:16px;
    padding:18px 18px 16px;
    box-shadow: var(--pi-shadow);

    position:relative;
    overflow:hidden;

    font: inherit;
    font-size: 1rem;
  }

  /* subtle accent line instead of a big border box */
  .pi-card::before{
    content:"";
    position:absolute;
    left:0;
    top:0;
    bottom:0;
    width:4px;
    background: linear-gradient(180deg, var(--pi-green), rgba(46,111,64,.25));
  }

  /* --- Section headers (no pills, no boxes) --- */
  .pi-card h3{
    margin:0 0 10px 0;
    padding-left:10px; /* align with content after accent line */
    font: inherit;
    font-weight:800;
    font-size:1.12rem;
    line-height:1.25;
    letter-spacing:.2px;
  }

  /* optional: small subtitle under h3 when you want it */
  .pi-subtitle{
    margin:-4px 0 12px 0;
    padding-left:10px;
    color: var(--pi-muted);
    font-size: 0.92rem;
  }

  .pi-card p{ margin:0 0 12px 0; padding-left:10px; }
  .pi-card p:last-child{ margin-bottom:0; }

  /* Lists */
  .pi-card ul{ margin:10px 0 0 28px; }
  .pi-card li{ margin:8px 0; }

  /* Links */
  .pi-card a, .pi-archived a{
    color: var(--pi-orange);
    text-decoration:none;
    font-weight:650;
  }
  .pi-card a:hover, .pi-archived a:hover{ text-decoration:underline; }

  /* Grid spans */
  .span-12{ grid-column: span 12; }
  .span-8{ grid-column: span 8; }
  .span-4{ grid-column: span 4; }

  /* Scroll area */
  .pi-scroll{
    max-height: 420px;
    overflow:auto;
    padding-right:6px;
  }

  /* Archived note: no box, just a clean muted line */
  .pi-archived{
    margin: 0 0 18px 0;
    padding: 0;
    color: var(--pi-muted);
    font: inherit;
    font-size: 0.95rem;
    line-height: 1.6;
  }
  .pi-archived strong{ color: var(--pi-text); }

  /* Make the hero card feel special (optional but nice) */
  .pi-hero{
    border-color: rgba(46,111,64,.28);
  }
  .pi-hero::after{
    content:"";
    position:absolute;
    right:-60px;
    top:-60px;
    width:180px;
    height:180px;
    background: radial-gradient(circle at 30% 30%, rgba(255,102,0,.18), transparent 60%);
    pointer-events:none;
  }
</style>


<p class="pi-archived">
  <strong>Archived page:</strong> A look into my Ph.D. years and journey before becoming a professor.
  For current updates, see <a href="/news/">Lab News</a> and <a href="/publications/">Publications</a>.
</p>
---

<div class="pi-grid">

  <!-- ABOUT / HERO -->
  <section class="pi-card span-12 pi-hero">
    <h3>University of Virginia | Computer Science</h3>
    <p class="pi-subtitle">Archived PhD timeline and highlights</p>

    <p>
      I earned my <strong>Ph.D. in Computer Science</strong> from the <strong>University of Virginia</strong> in Summer 2025, where I was advised by
      <a href="https://matthewbdwyer.github.io/">Dr. Matthew Dwyer</a>.
      Broadly, my research area is <strong>AI for Software Engineering</strong>, with a focus on <em>requirements, testing, debugging, and repair</em> for software systems.
      My long-term vision is to advance the development of high-quality, reliable software through <em>cost-effective automation</em> powered by <strong>AI/ML, large language models (LLMs),</strong> and <strong>agentic AI</strong>.
    </p>

    <p>
      During my Ph.D., I collaborated with <strong>Lockheed Martin</strong> and multiple teams at <strong>AWS</strong> (CodeGuru, CodeCatalyst, and AWS AI Labs),
      and my work has been published in premier venues including <strong>ICSE, FSE, and NeurIPS</strong>.
    </p>
  </section>

  <!-- EDUCATION -->
  <section class="pi-card span-12">
    <h3>Education</h3>
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
    <h3>Research Awards</h3>
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
    <h3>Service Award</h3>
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
    <h3>Travel Grants</h3>
    <ul>
      <li>ACM SIGSOFT travel grant - FSE'25, Trondheim, Norway.</li>
      <li>CRA travel grants - Grad Cohort (2023 San Francisco, 2020 New Orleans).</li>
      <li>The Society of Women Engineers (SWE)'24 - Chicago, IL (Oct 23-26, 2024).</li>
      <li>Grace Hopper Celebration (GHCI) - Bangalore, India (2015).</li>
    </ul>
  </section>

  <!-- UNDERGRAD ACADEMIC AWARDS -->
  <section class="pi-card span-12">
    <h3>Undergraduate Academic Awards</h3>
    <ul>
      <li><strong>Top Ten Database Project</strong>, CSE, BUET (2014)</li>
      <li><strong>Dean’s List (Level-2)</strong>, CSE, BUET (2013–2014)</li>
      <li><strong>University Merit Scholarship</strong>, CSE, BUET (2013–2014)</li>
    </ul>
  </section>

  <!-- NEWS (SCROLLABLE) -->
  <section class="pi-card span-12 pi-scroll">
    <h3>News</h3>
    <ul>
      <li><strong>August 1, 2025</strong>: Joined CS@UTD as a Tenure-track Assistant Professor.</li>
      <li><strong>July 25, 2025</strong>: Relocated to Dallas, TX from beautiful Virginia.</li>
      <li><strong>June 25, 2025</strong>: Attended FSE 2025 in Trondheim, Norway, and presented my paper <a href="https://dl.acm.org/doi/abs/10.1145/3729354">Doc2OracLL</a>.</li>
      <li><strong>April 25, 2025</strong>: Attended ICSE 2025 in Ottawa, Canada, and presented my paper <a href="https://ieeexplore.ieee.org/document/11029748">TOGLL</a>.</li>
      <li><strong>April 25, 2025</strong>: Successfully defended my Ph.D. and officially became Dr. Soneya Binta Hossain!</li>
      <li><strong>April 2025</strong>: My paper <a href="https://dl.acm.org/doi/abs/10.1145/3729354">Doc2Oracle: Investigating the Impact of Javadoc Comments on Test Oracle Generation</a> was accepted at FSE'25 Research Track.</li>
      <li><strong>November 2024</strong>: My paper <a href="https://ieeexplore.ieee.org/document/11029748">TOGLL: Correct and Strong Test Oracle Generation with LLMs</a> was accepted at ICSE'25 Research Track.</li>
      <li><strong>September 2024</strong>: Received a travel grant to attend SWE24 - the world’s largest conference for women in engineering and technology - held October 23-26 in Chicago, IL.</li>
      <li><strong>September 2024</strong>: Received UVA’s most prestigious Endowed Fellowship, awarded to outstanding doctoral students with a $12,000 stipend.</li>
      <li><strong>May 2024</strong>: Received Master of Computer Science (MCS) from UVA with a CGPA of 4.0/4.0. <a href="{{ '/graduation/' | relative_url }}">[gallery]</a></li>
      <li><strong>May 2024</strong>: Defended my Ph.D. dissertation proposal, titled <em>Assessing and Improving Critical Properties of Test Oracles for Effective Software Bug Detection</em>. <a href="{{ '/proposal/' | relative_url }}">[gallery]</a></li>
      <li><strong>April 2024</strong>: Attended ICSE 2024 in Lisbon, Portugal, and presented my paper at the Doctoral Symposium. <a href="{{ '/icse-24/' | relative_url }}">[gallery]</a></li>
      <li><strong>April 2024</strong>: Honored to be selected as one of the five finalists at the UVA Research Computing Exhibition 2024.</li>
      <li><strong>April 2024</strong>: My paper <a href="https://dl.acm.org/doi/abs/10.1145/3660773">A Deep Dive into Large Language Models for Automated Bug Localization and Repair</a> was accepted at FSE'24 Research Track.</li>
      <li><strong>December 2023</strong>: My paper <a href="https://dl.acm.org/doi/10.1145/3639478.3639791">Ensuring Critical Properties of Test Oracles for Effective Bug Detection</a> was accepted at the ICSE'24 Doctoral Symposium.</li>
      <li><strong>December 2023</strong>: Presented our paper <a href="https://dl.acm.org/doi/pdf/10.1145/3611643.3616265">Neural-Based Test Oracle Generation: A Large-Scale Evaluation and Lessons Learned</a> at FSE'23 (Dec 3-9) in San Francisco, CA. <a href="{{ '/FSE-23/' | relative_url }}">[gallery]</a></li>
      <li><strong>October 2023</strong>: Honored to receive the <a href="https://engineering.virginia.edu/department/computer-science/blogs/2023-cs-research-symposium-highlights">Student Choice Research Award</a> at the UVA CS Research Symposium 2023.</li>
      <li><strong>July 2023</strong>: Our paper <a href="https://dl.acm.org/doi/abs/10.1145/3611643.3616265">Neural-Based Test Oracle Generation: A Large-Scale Evaluation and Lessons Learned</a> was accepted at the FSE'23 Research Track.</li>
      <li><strong>June 2023</strong>: Started summer internship with the AWS CodeCatalyst team in Santa Clara, CA.</li>
      <li><strong>May 2023</strong>: Presented our <a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10172745">paper</a> at ICSE'23 in Melbourne, Australia. <a href="{{ '/ICSE-23/' | relative_url }}">[gallery]</a></li>
      <li><strong>May 2023</strong>: Received the <a href="https://engineering.virginia.edu/department/computer-science/blogs/cs-department-end-year-award-recipients-2022-2023">John A. Stankovic Outstanding Graduate Research Award</a>. <a href="award-23.md">[gallery]</a></li>
      <li><strong>April 2023</strong>: Attended CRA Grad Cohort in San Francisco, CA. <a href="{{ '/CRA-SFO/' | relative_url }}">[gallery]</a></li>
      <li><strong>February 2023</strong>: Our research <a href="https://github.com/soneyahossain/hcc-gap-recommender">artifact</a> was accepted at the <a href="https://conf.researchr.org/details/icse-2023/icse-2023-artifact-evaluation/5/Artifact-Measuring-and-Mitigating-Gaps-in-Structural-Testing">ICSE 2023 Artifact Evaluation Track</a>.</li>
      <li><strong>December 2022</strong>: Our paper <a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10172745">Measuring and Mitigating Gaps in Structural Testing</a> was accepted at the ICSE'23 Technical Track.</li>
      <li><strong>May 2022</strong>: Started summer internship with the AWS CodeGuru team in Seattle, WA.</li>
      <li><strong>May 2022</strong>: Received the <a href="https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards">Outstanding Graduate Service Award</a>. <a href="{{ '/service-award/' | relative_url }}">[gallery]</a></li>
      <li><strong>April 2022</strong>: Attended ICSE'22 in Pittsburgh, PA.</li>
      <li><strong>December 2021</strong>: Received the <a href="https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards">Outstanding Research Poster Award</a> at the CS Research Symposium.</li>
      <li><strong>December 2021</strong>: Organized the <a href="https://uvaeng.prod.acquia-sites.com/events/2021-fall-cs-research-symposium">CS Department Research Symposium</a>; see the <a href="https://engineering.virginia.edu/labs-groups/link-lab/blogs/computer-science-graduate-student-group-research-symposium">news</a> and <a href="https://twitter.com/CS_UVA/status/1471529342912155650?s=20&t=YbVecueDVPOLsdDaw0sBfQ">tweet</a>.</li>
      <li><strong>September 2021</strong>: Passed the Ph.D. Qualifying Exam with flying colors!</li>
      <li><strong>April 2021</strong>: Attended the CRA-W Grad Cohort Workshop 2021 (virtual, due to COVID-19).</li>
      <li><strong>February 2021</strong>: Started working as a TA for Graduate Compilers (CS 6620) with Prof. Matt Dwyer.</li>
      <li><strong>August 2019</strong>: Began Ph.D. in Computer Science at the University of Virginia.</li>
    </ul>
  </section>

</div>
