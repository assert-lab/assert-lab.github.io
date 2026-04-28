---
layout: single
permalink: /PI/
classes: wide
title: ""
author_profile: true
---

<style>
  :root{
    --pi-green:#2E6F40;
    --pi-orange:#c75b12;
    --pi-uva-blue:#232D4B;
    --pi-uva-orange:#E57200;
    --pi-ink:#1f2937;
    --pi-muted:#6b7280;
    --pi-line:rgba(46,111,64,.18);
    --pi-soft:#f8faf9;
    --pi-phd-soft:#fff8f1;
    --pi-shadow:0 12px 30px rgba(0,0,0,.06);
  }

  .pi-page{
    color:var(--pi-ink);
    font:inherit;
    font-size:0.98rem;
    line-height:1.65;
  }

  .pi-page a{
    color:var(--pi-orange);
    text-decoration:none;
    font-weight:700;
  }

  .pi-page a:hover{ text-decoration:underline; }

  .pi-hero{
    position:relative;
    overflow:hidden;
    border:1px solid var(--pi-line);
    border-radius:24px;
    padding:30px 32px;
    margin-bottom:20px;
    background:
      radial-gradient(circle at 88% 8%, rgba(199,91,18,.16), transparent 34%),
      linear-gradient(135deg,#ffffff 0%,#fbfdfb 72%,rgba(46,111,64,.07) 100%);
    box-shadow:var(--pi-shadow);
  }

  .pi-kicker{
    margin:0 0 8px 0;
    color:var(--pi-green);
    text-transform:uppercase;
    letter-spacing:.08em;
    font-weight:850;
    font-size:.78rem;
  }

  .pi-hero h1{
    margin:0 0 8px 0;
    font-size:2.25rem;
    line-height:1.1;
    letter-spacing:-.035em;
  }

  .pi-title{
    margin:0 0 14px 0;
    color:#374151;
    font-weight:650;
    font-size:1.05rem;
  }

  .pi-summary{
    max-width:1040px;
    margin:0 0 16px 0;
    font-size:1.03rem;
  }

  .pi-actions{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
    margin-top:16px;
  }

  .pi-button{
    display:inline-flex;
    align-items:center;
    gap:6px;
    border:1px solid rgba(46,111,64,.25);
    border-radius:999px;
    padding:7px 12px;
    text-decoration:none !important;
    font-weight:760;
    color:var(--pi-green) !important;
    background:#fff;
  }

  .pi-button.primary{
    color:#fff !important;
    background:var(--pi-green);
    border-color:var(--pi-green);
  }

  .pi-note{
    margin:12px 0 0 0;
    color:var(--pi-muted);
    font-size:.92rem;
  }

  .pi-grid{
    display:grid;
    grid-template-columns:repeat(12,1fr);
    gap:18px;
    align-items:start;
  }

  .pi-card{
    grid-column:span 6;
    position:relative;
    overflow:hidden;
    border:1px solid var(--pi-line);
    border-radius:18px;
    background:#fff;
    box-shadow:var(--pi-shadow);
    padding:20px 20px 18px 22px;
  }

  .pi-card::before{
    content:"";
    position:absolute;
    left:0;
    top:0;
    bottom:0;
    width:4px;
    background:linear-gradient(180deg,var(--pi-green),rgba(199,91,18,.34));
  }

  .pi-span-12{ grid-column:span 12; }
  .pi-span-8{ grid-column:span 8; }
  .pi-span-4{ grid-column:span 4; }
  .pi-span-6{ grid-column:span 6; }

  .pi-card h2,
  .pi-card h3{
    margin:0 0 10px 0;
    font-weight:850;
    line-height:1.25;
    letter-spacing:-.01em;
  }

  .pi-card h2{ font-size:1.22rem; }
  .pi-card h3{ font-size:1.08rem; }
  .pi-card p{ margin:0 0 12px 0; }
  .pi-card p:last-child{ margin-bottom:0; }
  .pi-card ul{ margin:8px 0 0 22px; }
  .pi-card li{ margin:7px 0; }

  .pi-tag-row{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
    margin:12px 0 0 0;
  }

  .pi-tag{
    display:inline-flex;
    align-items:center;
    border:1px solid rgba(46,111,64,.20);
    border-radius:999px;
    padding:4px 9px;
    background:var(--pi-soft);
    color:#334155;
    font-size:.88rem;
    font-weight:650;
  }

  .pi-mini-list{
    list-style:none;
    margin:10px 0 0 0 !important;
    padding:0;
  }

  .pi-mini-list li{
    margin:9px 0;
    padding-left:0;
  }

  .pi-date{
    display:inline-block;
    min-width:98px;
    color:var(--pi-muted);
    font-weight:800;
    font-size:.9rem;
  }

  .pi-callout{
    border-left:4px solid var(--pi-orange);
    background:#fff8f2;
    padding:12px 14px;
    border-radius:12px;
    margin:12px 0;
  }

  .pi-scroll{
    max-height:430px;
    overflow:auto;
    padding-right:8px;
  }

  .pi-muted{ color:var(--pi-muted); }

  .pi-section-divider{
    margin:26px 0 18px 0;
    padding:18px 20px;
    border-radius:18px;
    border:1px solid rgba(35,45,75,.18);
    background:linear-gradient(135deg,rgba(35,45,75,.07),rgba(229,114,0,.08));
  }

  .pi-section-divider h2{
    margin:0 0 6px 0;
    color:var(--pi-uva-blue);
    font-size:1.35rem;
    letter-spacing:-.02em;
  }

  .pi-section-divider p{
    margin:0;
    color:#4b5563;
  }

  .pi-phd-card{
    border-color:rgba(35,45,75,.18);
    background:linear-gradient(180deg,#fff,var(--pi-phd-soft));
  }

  .pi-phd-card::before{
    background:linear-gradient(180deg,var(--pi-uva-blue),var(--pi-uva-orange));
  }

  .pi-phd-card h2,
  .pi-phd-card h3{ color:var(--pi-uva-blue); }

  .pi-tableish{
    display:grid;
    grid-template-columns:160px 1fr;
    gap:8px 14px;
    margin-top:8px;
  }

  .pi-tableish strong{ color:#111827; }

  @media (max-width:1024px){
    .pi-grid{ grid-template-columns:repeat(6,1fr); }
    .pi-span-12,.pi-span-8,.pi-span-4,.pi-span-6,.pi-card{ grid-column:span 6; }
  }

  @media (max-width:640px){
    .pi-hero{ padding:22px 20px; }
    .pi-hero h1{ font-size:1.82rem; }
    .pi-grid{ grid-template-columns:repeat(2,1fr); }
    .pi-span-12,.pi-span-8,.pi-span-4,.pi-span-6,.pi-card{ grid-column:span 2; }
    .pi-tableish{ grid-template-columns:1fr; }
    .pi-date{ display:block; min-width:0; }
  }
</style>

<div class="pi-page">

  <section class="pi-hero" id="top">
    <p class="pi-kicker">Principal Investigator, AS²ERT Lab</p>
    <h1>Dr. Soneya Binta Hossain</h1>
    <p class="pi-title">
      Assistant Professor · Department of Computer Science · The University of Texas at Dallas
    </p>
    <p class="pi-summary">
      I lead the <strong>AS²ERT Lab</strong> — <em>AI for Safe Software Engineering and Testing</em>. We develop automated techniques to improve the safety and reliability of software systems, with research spanning <strong>software engineering</strong>, <strong>program analysis</strong>, <strong>software testing</strong>, <strong>debugging</strong>, <strong>bug localization</strong>, and <strong>repair</strong>. A major focus of my group is responsibly integrating modern AI methods, including <strong>large language models</strong> and <strong>agentic systems</strong>, into automated software engineering workflows.
    </p>
    <p class="pi-summary">
      Before joining UT Dallas, I earned my Ph.D. and M.S. in Computer Science from the University of Virginia, where I worked with <a href="https://matthewbdwyer.github.io/">Prof. Matthew Dwyer</a> on AI-driven software testing and test oracle generation. I earned my B.Sc. in Computer Science and Engineering from BUET.
    </p>
    <div class="pi-actions">
      <a class="pi-button primary" href="#working-with-me">Work with me</a>
      <a class="pi-button" href="#research">Research</a>
      <a class="pi-button" href="#publications">Publications</a>
      <a class="pi-button" href="#service">Service</a>
      <a class="pi-button" href="#phd-archive">Ph.D. archive</a>
      <a class="pi-button" href="mailto:sbhossain@utdallas.edu">Email</a>
    </div>
    <p class="pi-note">Currently accepting undergraduate and graduate students. Last updated: {{ site.time | date: "%B %Y" }}.</p>
  </section>

  <div class="pi-grid">

    <section class="pi-card pi-span-4">
      <h2>Contact</h2>
      <ul class="pi-mini-list">
        <li><strong>Office:</strong> ECS 4.231</li>
        <li><strong>Phone:</strong> +1 (972) 883-4172</li>
        <li><strong>Email:</strong> <a href="mailto:sbhossain@utdallas.edu">sbhossain@utdallas.edu</a></li>
        <li><strong>Location:</strong> Dallas, TX, USA</li>
        <li><a href="https://profiles.utdallas.edu/sbhossain">UTD Profile</a> · <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ">Google Scholar</a></li>
        <li><a href="https://github.com/soneyahossain">GitHub</a> · <a href="https://www.linkedin.com/in/soneya/">LinkedIn</a> · <a href="https://orcid.org/0000-0002-7282-061X">ORCID</a></li>
      </ul>
    </section>

    <section class="pi-card pi-span-12" id="research">
      <h2>Research interests</h2>
      <p>
        AS²ERT develops techniques, datasets, and benchmarks for safe, reliable, and trustworthy software systems. My research is especially interested in when AI-for-software-engineering systems work, when they fail, and how to evaluate them rigorously.
      </p>
      <div class="pi-tag-row">
        <span class="pi-tag">Trustworthy AI for Software Engineering</span>
        <span class="pi-tag">Automated Testing</span>
        <span class="pi-tag">Test Oracles</span>
        <span class="pi-tag">Bug Localization</span>
        <span class="pi-tag">Debugging & Repair</span>
        <span class="pi-tag">Program Analysis</span>
        <span class="pi-tag">Datasets & Benchmarks</span>
        <span class="pi-tag">Quantum Software Testing</span>
      </div>
      <ul>
        <li><strong>LLMs for software testing:</strong> generating correct, strong, and useful test oracles and measuring what makes oracle generation succeed or fail.</li>
        <li><strong>Reliable AI coding systems:</strong> studying how LLMs localize, debug, repair, and explain software defects.</li>
        <li><strong>Benchmarks and empirical evidence:</strong> building datasets and evaluation methods that make AI-for-SE progress measurable and reproducible.</li>
        <li><strong>Safe software engineering automation:</strong> combining AI with program analysis, testing, and human-centered evaluation.</li>
      </ul>
    </section>

    
   
    <section class="pi-card pi-span-6">
      <h2>Teaching</h2>
      <ul>
        <li><strong>CS/CE/SE 3354 — Software Engineering</strong>, Fall 2025. Course coordinator.</li>
        <li><strong>CS/SE 6356 — Software Maintenance, Evolution & Re-engineering</strong>, Spring 2026. Cross-listed with SYSM 6308.</li>
        <li><strong>Graduate Teaching Assistant, UVA</strong>, 2021–2023: CS 4620 Undergraduate Compilers and CS 6620 Graduate Compilers; guest lectures in compilers and program analysis.</li>
      </ul>
      <p><a href="{{ '/teaching/' | relative_url }}">Lab teaching page →</a></p>
    </section>

   

    <section class="pi-card pi-span-12" id="service">
      <h2>Service</h2>
      <p>
        I view service as part of building a healthier research community: reviewing carefully, supporting students, organizing events that create opportunities, and helping broaden participation in computing.
      </p>
      <div class="pi-grid" style="margin-top:8px;">
        <section class="pi-card pi-span-6">
          <h3>Program committees and reviewing</h3>
          <ul>
            <li><strong>SPLASH/ISSTA 2026</strong> Social Events Co-Chair in Organizing Committee.</li>
            <li><strong>FSE 2027</strong>, ACM International Conference on the Foundations of Software Engineering.</li>
            <li><strong>ASE 2026</strong>, Tools and Datasets Track, IEEE/ACM International Conference on Automated Software Engineering.</li>
            <li><strong>FSE 2026</strong>, Ideas, Visions and Reflections Track.</li>
            <li><strong>AIware 2026</strong>, ACM International Conference on AI-Powered Software.</li>
            <li><strong>ICST 2026</strong>, IEEE International Conference on Software Testing, Verification and Validation.</li>
            <li><strong>ICST 2024</strong>, Research Track, IEEE International Conference on Software Testing, Verification and Validation.</li>
            <li><strong>ACM TOSEM</strong>, reviewing service.</li>
          </ul>
        </section>
        <section class="pi-card pi-span-6">
          <h3>Conference and professional service</h3>
          <ul>
            <li><strong>Recruiter</strong>, SWE24, Chicago, IL. Assisted UVA Engineering with recruiting, booth setup, and outreach.</li>
            <li><strong>Student Volunteer</strong>, ESEC/FSE 2023, San Francisco, CA. Assisted with registration, badge verification, presentation testing, A/V setup, and event preparation.</li>
            <li><strong>Travel-grant recipient and participant</strong>, CRA Grad Cohort, SWE, and Grace Hopper Celebration India.</li>
          </ul>
        </section>
        <section class="pi-card pi-span-6">
          <h3>Departmental and lab service</h3>
          <ul>
            <li><strong>Course coordinator</strong>, CS/CE/SE 3354 Software Engineering, UT Dallas CS.</li>
            <li><strong>Faculty mentor</strong>, AS²ERT Lab undergraduate research projects through RIDE and URAP.</li>
            <li><strong>Leadership Chair</strong>, Computer Science Graduate Student Group, UVA, Jan 2020–Jan 2022.</li>
            <li><strong>Organizer</strong>, UVA CS Research Symposium, 2020 and 2021.</li>
            <li>Assisted UVA CS with faculty recruitment and graduate student visits.</li>
          </ul>
        </section>
        <section class="pi-card pi-span-6">
          <h3>Mentoring and outreach</h3>
          <ul>
            <li><strong>Undergraduate research mentor</strong>, more than 10 students from universities in the U.S. and Bangladesh.</li>
            <li><strong>BWCSE Mentor</strong>, Bangladeshi Women in Computer Science and Engineering; mentored BUET students preparing for research and graduate school.</li>
            <li><strong>Social Chair</strong>, Association of Bangladeshi Students at UVA, Fall 2021–Summer 2022.</li>
            <li><strong>Service awards:</strong> Grace Hopper Spirit Award, UTD CS, 2025; Outstanding Graduate Service Award, UVA CS, 2022.</li>
          </ul>
        </section>
      </div>
    </section>

    <section class="pi-card pi-span-6">
      <h2>Education</h2>
      <ul>
        <li><strong>Ph.D., Computer Science</strong>, University of Virginia.<br>
          Advisor: Matthew Dwyer. Dissertation: <em>Assessing and Improving Critical Properties of Test Oracles for Effective Software Bug Detection.</em>
        </li>
        <li><strong>MCS, Computer Science</strong>, University of Virginia.<br>
          Project: <em>TOGLL: Correct and Strong Test Oracle Generation with LLMs.</em>
        </li>
        <li><strong>B.Sc., Computer Science and Engineering</strong>, Bangladesh University of Engineering and Technology (BUET).<br>
          Thesis: <em>Balanced Coverage in Fault-Tolerant Broadcasting for Wireless Multi-hop Networks.</em>
        </li>
      </ul>
    </section>

    <section class="pi-card pi-span-6">
      <h2>Selected honors and awards</h2>
      <ul>
        <li><strong>Grace Hopper Spirit Award</strong>, UTD CS, 2025.</li>
        <li><strong>Copenhaver Charitable Trust Bicentennial Fellow</strong>, UVA, 2024–2025.</li>
        <li><strong>John A. Stankovic Outstanding Graduate Research Award</strong>, UVA CS, 2023.</li>
        <li><strong>Student Choice Best Research Award</strong>, UVA CS Research Symposium, 2023.</li>
        <li><strong>Outstanding Graduate Service Award</strong>, UVA CS, 2022.</li>
        <li><strong>Best Research Poster</strong>, UVA CS Research Symposium, 2021.</li>
      </ul>
    </section>


  </div>

  <section class="pi-section-divider" id="phd-archive">
    <h2>Ph.D. journey and achievements</h2>
    <p>
      This section intentionally preserves my graduate-school story in a separate style. It keeps the awards, service, travel, teaching, mentoring, research milestones, and conference history from my Ph.D. life while the top of the page emphasizes my current faculty and lab role.
    </p>
  </section>

  <div class="pi-grid">

    <section class="pi-card pi-phd-card pi-span-12">
      <h2>University of Virginia · Computer Science</h2>
      <p>
        I earned my <strong>Ph.D. in Computer Science</strong> from the <strong>University of Virginia</strong> in Summer 2025, advised by <a href="https://matthewbdwyer.github.io/">Dr. Matthew Dwyer</a>. Broadly, my Ph.D. research focused on <strong>AI for Software Engineering</strong>, especially <em>requirements, testing, debugging, and repair</em> for software systems. My long-term vision during the Ph.D. was to advance the development of high-quality, reliable software through <em>cost-effective automation</em> powered by <strong>AI/ML</strong>, <strong>LLMs</strong>, and <strong>agentic AI</strong>.
      </p>
      <p>
        During my Ph.D., I collaborated with <strong>Lockheed Martin</strong> and multiple teams at <strong>AWS</strong> — CodeGuru, CodeCatalyst, and AWS AI Labs — and published work in premier venues including <strong>ICSE</strong>, <strong>FSE</strong>, and <strong>NeurIPS</strong>.
      </p>
    </section>

    <section class="pi-card pi-phd-card pi-span-12">
      <h2>Ph.D. education details</h2>
      <div class="pi-tableish">
        <strong>Ph.D.</strong>
        <span>Computer Science, University of Virginia. Advisor: Matthew Dwyer. Committee: Sebastian Elbaum, Yangfeng Ji, Matthew Bolton, Antonio Filieri. Thesis: <em>Assessing and Improving Critical Properties of Test Oracles for Effective Software Bug Detection.</em></span>
        <strong>MCS</strong>
        <span>Computer Science, University of Virginia. Project: <em>TOGLL: Correct and Strong Test Oracle Generation with LLMs.</em> CGPA: 4.0/4.0.</span>
        <strong>B.Sc.</strong>
        <span>Computer Science and Engineering, BUET. Thesis: <em>Balanced Coverage in Fault-Tolerant Broadcasting for Wireless Multi-hop Networks.</em></span>
      </div>
    </section>

    <section class="pi-card pi-phd-card pi-span-6">
      <h2>Ph.D. research awards</h2>
      <ul>
        <li><strong>Copenhaver Charitable Trust Bicentennial Fellow</strong>, UVA School of Engineering & Applied Science, 2024–2025, awarded $12,000.</li>
        <li><strong>Finalist</strong>, Physical Sciences and Engineering Category, UVA Research Computing Exhibition 2024, showcasing work using UVA’s Rivanna high-performance computing resources.</li>
        <li><strong>John A. Stankovic Outstanding Graduate Research Award</strong>, CS, UVA, 2022–2023. <a href="https://engineering.virginia.edu/department/computer-science/blogs/cs-department-end-year-award-recipients-2022-2023">[link]</a></li>
        <li><strong>Student Choice Best Research Award</strong>, 2023 CS Research Symposium, UVA. <a href="https://engineering.virginia.edu/department/computer-science/blogs/2023-cs-research-symposium-highlights">[link]</a></li>
        <li><strong>Best Research Poster Award</strong>, 2021 CS Research Symposium, UVA. <a href="https://uvaeng.prod.acquia-sites.com/events/2021-fall-cs-research-symposium">[link]</a></li>
        <li><strong>Ph.D. Fellowship</strong>, Department of Computer Science, University of Virginia, 2019.</li>
        <li><strong>Outstanding Undergraduate Thesis Award</strong>, Department of CSE, BUET, 2016.</li>
      </ul>
    </section>

    <section class="pi-card pi-phd-card pi-span-6">
      <h2>Service awards and leadership</h2>
      <ul>
        <li><strong>Outstanding Graduate Service Award</strong>, CS Department, University of Virginia, 2022. <a href="https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards">[link]</a></li>
        <li><strong>Leadership Chair</strong>, Computer Science Graduate Student Group (CSGSG), UVA, Jan 2020–Jan 2022.</li>
        <li>Organized leadership and social events and served as a bridge between graduate students and the department.</li>
        <li><strong>Organizer</strong>, UVA CS Research Symposium in 2020 and 2021.</li>
        <li><strong>Social Chair</strong>, Association of Bangladeshi Students (ABS), UVA, Fall 2021–Summer 2022.</li>
      </ul>
    </section>

    <section class="pi-card pi-phd-card pi-span-6">
      <h2>Travel grants</h2>
      <ul>
        <li><strong>ACM SIGSOFT travel grant</strong> to attend FSE 2025 in Trondheim, Norway.</li>
        <li><strong>Society of Women Engineers SWE24 travel grant</strong>, Chicago, IL, October 23–26, 2024.</li>
        <li><strong>CRA Grad Cohort travel grant</strong>, San Francisco, CA, 2023.</li>
        <li><strong>CRA Grad Cohort travel grant</strong>, New Orleans, LA, 2020.</li>
        <li><strong>Grace Hopper Celebration India travel grant</strong>, Bangalore, India, 2015.</li>
      </ul>
    </section>

    <section class="pi-card pi-phd-card pi-span-6">
      <h2>Undergraduate academic awards</h2>
      <ul>
        <li><strong>Top Ten Database Project Award</strong>, Department of CSE, BUET, 2014.</li>
        <li><strong>Dean’s List Award</strong>, Level 2, Department of CSE, BUET, 2013–2014.</li>
        <li><strong>University Merit Scholarship</strong>, Department of CSE, BUET, 2013–2014.</li>
      </ul>
    </section>

    <section class="pi-card pi-phd-card pi-span-6">
      <h2>Ph.D.-era teaching and mentoring</h2>
      <ul>
        <li><strong>Graduate TA</strong>, CS 4620 Undergraduate Compilers and CS 6620 Graduate Compilers, UVA.</li>
        <li>Guest lectures in compilers and program analysis.</li>
        <li><strong>Student mentor</strong>, University of Virginia: mentored undergraduate students from universities in the U.S. and Bangladesh, focusing on research and graduate school preparation.</li>
        <li><strong>Mentees included:</strong> Raygan Taylor, Javan Mendoza, Nicki Choquette, Kasra Lekan, Ashley Hart, Srikar Chittari, and Eric Weng.</li>
        <li><strong>BWCSE Mentor:</strong> mentored Bangladeshi women in CSE, including BUET students preparing for research and graduate school.</li>
      </ul>
    </section>

    <section class="pi-card pi-phd-card pi-span-6">
      <h2>Internships and collaborations</h2>
      <ul>
        <li><strong>AWS CodeCatalyst</strong>, Santa Clara, CA, Summer 2023.</li>
        <li><strong>AWS CodeGuru</strong>, Seattle, WA, Summer 2022.</li>
        <li><strong>AWS AI Labs</strong>, research collaboration during Ph.D. work.</li>
        <li><strong>Lockheed Martin</strong>, research collaboration during Ph.D. work.</li>
      </ul>
    </section>

    <section class="pi-card pi-phd-card pi-span-12 pi-scroll">
      <h2>Ph.D. timeline and archived news</h2>
      <ul class="pi-mini-list">
        <li><span class="pi-date">Aug 1, 2025</span> Joined CS@UTD as a tenure-track Assistant Professor.</li>
        <li><span class="pi-date">Jul 25, 2025</span> Relocated to Dallas, TX from Virginia.</li>
        <li><span class="pi-date">Jun 25, 2025</span> Attended FSE 2025 in Trondheim, Norway, and presented <a href="https://dl.acm.org/doi/abs/10.1145/3729354">Doc2OracLL</a>.</li>
        <li><span class="pi-date">Apr 25, 2025</span> Attended ICSE 2025 in Ottawa, Canada, and presented <a href="https://ieeexplore.ieee.org/document/11029748">TOGLL</a>.</li>
        <li><span class="pi-date">Apr 25, 2025</span> Successfully defended my Ph.D. dissertation and officially became Dr. Soneya Binta Hossain.</li>
        <li><span class="pi-date">Apr 2025</span> <a href="https://dl.acm.org/doi/abs/10.1145/3729354">Doc2Oracle: Investigating the Impact of Javadoc Comments on Test Oracle Generation</a> was accepted to the FSE 2025 Research Track.</li>
        <li><span class="pi-date">Nov 2024</span> <a href="https://ieeexplore.ieee.org/document/11029748">TOGLL: Correct and Strong Test Oracle Generation with LLMs</a> was accepted to the ICSE 2025 Research Track.</li>
        <li><span class="pi-date">Sep 2024</span> Received a travel grant to attend SWE24, the world’s largest conference for women in engineering and technology, held October 23–26 in Chicago, IL.</li>
        <li><span class="pi-date">Sep 2024</span> Received UVA’s Copenhaver Charitable Trust Bicentennial Fellowship, an endowed fellowship awarded to outstanding doctoral students with a $12,000 stipend.</li>
        <li><span class="pi-date">May 2024</span> Received Master of Computer Science from UVA with a CGPA of 4.0/4.0. <a href="{{ '/graduation/' | relative_url }}">[gallery]</a></li>
        <li><span class="pi-date">May 2024</span> Defended my Ph.D. dissertation proposal, titled <em>Assessing and Improving Critical Properties of Test Oracles for Effective Software Bug Detection</em>. <a href="{{ '/proposal/' | relative_url }}">[gallery]</a></li>
        <li><span class="pi-date">Apr 2024</span> Attended ICSE 2024 in Lisbon, Portugal, and presented my paper at the Doctoral Symposium. <a href="{{ '/icse-24/' | relative_url }}">[gallery]</a></li>
        <li><span class="pi-date">Apr 2024</span> Selected as one of five finalists at the UVA Research Computing Exhibition 2024.</li>
        <li><span class="pi-date">Apr 2024</span> <a href="https://dl.acm.org/doi/abs/10.1145/3660773">A Deep Dive into Large Language Models for Automated Bug Localization and Repair</a> was accepted to the FSE 2024 Research Track.</li>
        <li><span class="pi-date">Dec 2023</span> <a href="https://dl.acm.org/doi/10.1145/3639478.3639791">Ensuring Critical Properties of Test Oracles for Effective Bug Detection</a> was accepted to the ICSE 2024 Doctoral Symposium.</li>
        <li><span class="pi-date">Dec 2023</span> Presented <a href="https://dl.acm.org/doi/pdf/10.1145/3611643.3616265">Neural-Based Test Oracle Generation: A Large-Scale Evaluation and Lessons Learned</a> at FSE 2023 in San Francisco, CA. <a href="{{ '/FSE-23/' | relative_url }}">[gallery]</a></li>
        <li><span class="pi-date">Oct 2023</span> Received the <a href="https://engineering.virginia.edu/department/computer-science/blogs/2023-cs-research-symposium-highlights">Student Choice Research Award</a> at the UVA CS Research Symposium 2023.</li>
        <li><span class="pi-date">Jul 2023</span> <a href="https://dl.acm.org/doi/abs/10.1145/3611643.3616265">Neural-Based Test Oracle Generation: A Large-Scale Evaluation and Lessons Learned</a> was accepted to the FSE 2023 Research Track.</li>
        <li><span class="pi-date">Jun 2023</span> Started summer internship with the AWS CodeCatalyst team in Santa Clara, CA.</li>
        <li><span class="pi-date">May 2023</span> Presented our <a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10172745">ICSE 2023 paper</a> in Melbourne, Australia. <a href="{{ '/ICSE-23/' | relative_url }}">[gallery]</a></li>
        <li><span class="pi-date">May 2023</span> Received the <a href="https://engineering.virginia.edu/department/computer-science/blogs/cs-department-end-year-award-recipients-2022-2023">John A. Stankovic Outstanding Graduate Research Award</a>. <a href="{{ '/award-23/' | relative_url }}">[gallery]</a></li>
        <li><span class="pi-date">Apr 2023</span> Attended CRA Grad Cohort in San Francisco, CA. <a href="{{ '/CRA-SFO/' | relative_url }}">[gallery]</a></li>
        <li><span class="pi-date">Feb 2023</span> Our research <a href="https://github.com/soneyahossain/hcc-gap-recommender">artifact</a> was accepted at the <a href="https://conf.researchr.org/details/icse-2023/icse-2023-artifact-evaluation/5/Artifact-Measuring-and-Mitigating-Gaps-in-Structural-Testing">ICSE 2023 Artifact Evaluation Track</a>.</li>
        <li><span class="pi-date">Dec 2022</span> <a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10172745">Measuring and Mitigating Gaps in Structural Testing</a> was accepted to the ICSE 2023 Technical Track.</li>
        <li><span class="pi-date">May 2022</span> Started summer internship with the AWS CodeGuru team in Seattle, WA.</li>
        <li><span class="pi-date">May 2022</span> Received the <a href="https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards">Outstanding Graduate Service Award</a>. <a href="{{ '/service-award/' | relative_url }}">[gallery]</a></li>
        <li><span class="pi-date">Apr 2022</span> Attended ICSE 2022 in Pittsburgh, PA.</li>
        <li><span class="pi-date">Dec 2021</span> Received the <a href="https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards">Outstanding Research Poster Award</a> at the CS Research Symposium.</li>
        <li><span class="pi-date">Dec 2021</span> Organized the <a href="https://uvaeng.prod.acquia-sites.com/events/2021-fall-cs-research-symposium">CS Department Research Symposium</a>; see the <a href="https://engineering.virginia.edu/labs-groups/link-lab/blogs/computer-science-graduate-student-group-research-symposium">news</a> and <a href="https://twitter.com/CS_UVA/status/1471529342912155650?s=20&t=YbVecueDVPOLsdDaw0sBfQ">tweet</a>.</li>
        <li><span class="pi-date">Sep 2021</span> Passed the Ph.D. qualifying exam.</li>
        <li><span class="pi-date">Apr 2021</span> Attended the CRA-W Grad Cohort Workshop 2021 virtually.</li>
        <li><span class="pi-date">Feb 2021</span> Started working as a TA for Graduate Compilers, CS 6620, with Prof. Matt Dwyer.</li>
        <li><span class="pi-date">Aug 2019</span> Began Ph.D. in Computer Science at the University of Virginia.</li>
      </ul>
    </section>

  </div>

</div>
