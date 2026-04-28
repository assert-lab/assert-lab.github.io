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
    --pi-soft:#f8faf9;
    --pi-line:rgba(46,111,64,.18);
    --pi-archive-line:rgba(35,45,75,.18);
    --pi-shadow:0 12px 30px rgba(0,0,0,.055);
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
    margin-bottom:22px;
    background:
      radial-gradient(circle at 92% 8%, rgba(199,91,18,.16), transparent 34%),
      linear-gradient(135deg,#ffffff 0%,#fbfdfb 70%,rgba(46,111,64,.07) 100%);
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
    margin:0 0 14px 0;
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

  .pi-tag-row{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
    margin:14px 0 0 0;
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

  .pi-section{
    margin:24px 0;
  }

  .pi-section-title{
    margin:0 0 12px 0;
    font-size:1.32rem;
    line-height:1.25;
    letter-spacing:-.02em;
    color:#111827;
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

  .pi-card h3{
    margin:0 0 10px 0;
    font-weight:850;
    line-height:1.25;
    letter-spacing:-.01em;
    font-size:1.08rem;
  }

  .pi-card p{ margin:0 0 12px 0; }
  .pi-card p:last-child{ margin-bottom:0; }
  .pi-card ul{ margin:8px 0 0 22px; }
  .pi-card li{ margin:7px 0; }

  .pi-span-12{ grid-column:span 12; }
  .pi-span-8{ grid-column:span 8; }
  .pi-span-6{ grid-column:span 6; }
  .pi-span-4{ grid-column:span 4; }

  .pi-subtle{
    color:var(--pi-muted);
    font-size:.93rem;
  }

  .pi-course-meta{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
    margin:10px 0 12px 0;
  }

  .pi-course-meta a,
  .pi-course-meta span{
    display:inline-flex;
    align-items:center;
    border:1px solid rgba(46,111,64,.20);
    border-radius:999px;
    padding:3px 9px;
    background:var(--pi-soft);
    color:#334155 !important;
    font-size:.86rem;
    font-weight:700;
    text-decoration:none !important;
  }

  .pi-course-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:14px;
    margin-top:10px;
  }

  .pi-mini-box{
    border:1px solid rgba(46,111,64,.14);
    border-radius:14px;
    padding:12px 13px;
    background:#fbfdfb;
  }

  .pi-mini-box h4{
    margin:0 0 6px 0;
    font-size:.98rem;
    color:#111827;
  }

  .pi-mini-box ul{
    margin:6px 0 0 18px;
  }

  .pi-archive-intro{
    margin:28px 0 18px 0;
    padding:18px 20px;
    border-radius:18px;
    border:1px solid var(--pi-archive-line);
    background:linear-gradient(135deg,rgba(35,45,75,.07),rgba(229,114,0,.08));
  }

  .pi-archive-intro h2{
    margin:0 0 6px 0;
    color:var(--pi-uva-blue);
    font-size:1.35rem;
    letter-spacing:-.02em;
  }

  .pi-archive-intro p{
    margin:0;
    color:#4b5563;
  }

  .pi-archive-card{
    border-color:var(--pi-archive-line);
    background:linear-gradient(180deg,#fff,#fff8f1);
  }

  .pi-archive-card::before{
    background:linear-gradient(180deg,var(--pi-uva-blue),var(--pi-uva-orange));
  }

  .pi-archive-card h3{ color:var(--pi-uva-blue); }

  .pi-timeline{
    list-style:none;
    margin:10px 0 0 0 !important;
    padding:0;
  }

  .pi-timeline li{
    display:grid;
    grid-template-columns:112px 1fr;
    gap:10px;
    margin:9px 0;
    padding:0 0 9px 0;
    border-bottom:1px solid rgba(35,45,75,.10);
  }

  .pi-timeline li:last-child{
    border-bottom:0;
    padding-bottom:0;
  }

  .pi-date{
    color:var(--pi-muted);
    font-weight:800;
    font-size:.9rem;
  }

  @media (max-width:1024px){
    .pi-grid{ grid-template-columns:repeat(6,1fr); }
    .pi-span-12,.pi-span-8,.pi-span-6,.pi-span-4,.pi-card{ grid-column:span 6; }
  }

  @media (max-width:760px){
    .pi-course-grid{ grid-template-columns:1fr; }
  }

  @media (max-width:640px){
    .pi-hero{ padding:22px 20px; }
    .pi-hero h1{ font-size:1.82rem; }
    .pi-grid{ grid-template-columns:repeat(2,1fr); }
    .pi-span-12,.pi-span-8,.pi-span-6,.pi-span-4,.pi-card{ grid-column:span 2; }
    .pi-timeline li{ grid-template-columns:1fr; gap:2px; }
  }
</style>

<div class="pi-page">

  <section class="pi-hero" id="top">
    <p class="pi-kicker">Principal Investigator, AS²ERT Lab</p>
    <h1>Dr. Soneya Binta Hossain</h1>
    <p class="pi-title">Assistant Professor · Department of Computer Science · The University of Texas at Dallas</p>

    <p class="pi-summary">
      I lead the <strong>AS²ERT Lab</strong> — <em>AI for Safe Software Engineering and Testing</em>. We develop automated techniques to improve the safety and reliability of software systems, with research spanning <strong>software engineering</strong>, <strong>program analysis</strong>, <strong>software testing</strong>, <strong>debugging</strong>, <strong>bug localization</strong>, and <strong>repair</strong>. A major focus of my group is responsibly integrating modern AI methods, including <strong>large language models</strong> and <strong>agentic systems</strong>, into automated software engineering workflows.
    </p>

    <div class="pi-tag-row" aria-label="Research areas">
      <span class="pi-tag">Trustworthy AI for Software Engineering</span>
      <span class="pi-tag">Automated Testing</span>
      <span class="pi-tag">Test Oracles</span>
      <span class="pi-tag">Bug Localization</span>
      <span class="pi-tag">Debugging & Repair</span>
      <span class="pi-tag">Program Analysis</span>
      <span class="pi-tag">Datasets & Benchmarks</span>
      <span class="pi-tag">Quantum Software Testing</span>
    </div>

    <div class="pi-actions">
      <a class="pi-button primary" href="#education">Education</a>
      <a class="pi-button" href="#awards">Awards</a>
      <a class="pi-button" href="#service">Service</a>
      <a class="pi-button" href="#teaching">Teaching</a>
      <a class="pi-button" href="#phd-archive">Ph.D. Archive</a>
      <a class="pi-button" href="{{ '/news/' | relative_url }}">Lab News</a>
      <a class="pi-button" href="mailto:sbhossain@utdallas.edu">Email</a>
    </div>

    <p class="pi-note">Currently accepting undergraduate and graduate students. Last updated: {{ site.time | date: "%B %Y" }}.</p>
  </section>

  <section class="pi-section" id="education">
    <h2 class="pi-section-title">Education</h2>
    <div class="pi-grid">
      <section class="pi-card pi-span-8">
        <h3>Degrees</h3>
        <ul>
          <li><strong>Ph.D., Computer Science</strong>, University of Virginia.<br>
            Advisor: Matthew Dwyer. Committee: Sebastian Elbaum, Yangfeng Ji, Matthew Bolton, Antonio Filieri. Dissertation: <em>Assessing and Improving Critical Properties of Test Oracles for Effective Software Bug Detection.</em>
          </li>
          <li><strong>MCS, Computer Science</strong>, University of Virginia.<br>
            Project: <em>TOGLL: Correct and Strong Test Oracle Generation with LLMs.</em> CGPA: 4.0/4.0.
          </li>
          <li><strong>B.Sc., Computer Science and Engineering</strong>, Bangladesh University of Engineering and Technology (BUET).<br>
            Thesis: <em>Balanced Coverage in Fault-Tolerant Broadcasting for Wireless Multi-hop Networks.</em>
          </li>
        </ul>
      </section>

      <section class="pi-card pi-span-4">
        <h3>Professional Background</h3>
        <ul>
          <li><strong>Assistant Professor</strong>, Computer Science, UT Dallas, 2025–present.</li>
          <li><strong>AWS CodeCatalyst</strong>, Santa Clara, CA, Summer 2023.</li>
          <li><strong>AWS CodeGuru</strong>, Seattle, WA, Summer 2022.</li>
          <li><strong>Software Engineer II</strong>, REVE Systems, Dhaka, Bangladesh, 2016–2019.</li>
        </ul>
      </section>
    </div>
  </section>

  <section class="pi-section" id="awards">
    <h2 class="pi-section-title">Awards</h2>
    <div class="pi-grid">
      <section class="pi-card pi-span-6">
        <h3>Honors and Recognition</h3>
        <ul>
          <li><strong>Grace Hopper Spirit Award</strong>, UTD CS, 2025.</li>
          <li><strong>Copenhaver Charitable Trust Bicentennial Fellow</strong>, UVA School of Engineering & Applied Science, 2024–2025, awarded $12,000.</li>
          <li><strong>Finalist</strong>, Physical Sciences and Engineering Category, UVA Research Computing Exhibition 2024, showcasing work using UVA’s Rivanna high-performance computing resources.</li>
          <li><strong>John A. Stankovic Outstanding Graduate Research Award</strong>, CS, UVA, 2022–2023. <a href="https://engineering.virginia.edu/department/computer-science/blogs/cs-department-end-year-award-recipients-2022-2023">[link]</a></li>
          <li><strong>Student Choice Best Research Award</strong>, 2023 CS Research Symposium, UVA. <a href="https://engineering.virginia.edu/department/computer-science/blogs/2023-cs-research-symposium-highlights">[link]</a></li>
          <li><strong>Outstanding Graduate Service Award</strong>, CS Department, University of Virginia, 2022. <a href="https://uvaeng.prod.acquia-sites.com/2021-2022-cs-department-end-year-awards">[link]</a></li>
          <li><strong>Best Research Poster Award</strong>, 2021 CS Research Symposium, UVA. <a href="https://uvaeng.prod.acquia-sites.com/events/2021-fall-cs-research-symposium">[link]</a></li>
          <li><strong>Ph.D. Fellowship</strong>, Department of Computer Science, University of Virginia, 2019.</li>
          <li><strong>Outstanding Undergraduate Thesis Award</strong>, Department of CSE, BUET, 2016.</li>
        </ul>
      </section>

      <section class="pi-card pi-span-6">
        <h3>Travel Grants and Undergraduate Awards</h3>
        <ul>
          <li><strong>ACM SIGSOFT travel grant</strong> to attend FSE 2025 in Trondheim, Norway.</li>
          <li><strong>Society of Women Engineers SWE24 travel grant</strong>, Chicago, IL, October 23–26, 2024.</li>
          <li><strong>CRA Grad Cohort travel grant</strong>, San Francisco, CA, 2023.</li>
          <li><strong>CRA Grad Cohort travel grant</strong>, New Orleans, LA, 2020.</li>
          <li><strong>Grace Hopper Celebration India travel grant</strong>, Bangalore, India, 2015.</li>
          <li><strong>Top Ten Database Project Award</strong>, Department of CSE, BUET, 2014.</li>
          <li><strong>Dean’s List Award</strong>, Level 2, Department of CSE, BUET, 2013–2014.</li>
          <li><strong>University Merit Scholarship</strong>, Department of CSE, BUET, 2013–2014.</li>
        </ul>
      </section>
    </div>
  </section>

  <section class="pi-section" id="service">
    <h2 class="pi-section-title">Service</h2>
    <div class="pi-grid">
      <section class="pi-card pi-span-6">
        <h3>Program Committees and Reviewing</h3>
        <ul>
          <li><strong>SPLASH/ISSTA 2026</strong>, Social Events Co-Chair in Organizing Committee.</li>
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
        <h3>Departmental, Conference, and Outreach Service</h3>
        <ul>
          <li><strong>Leadership Chair</strong>, Computer Science Graduate Student Group, UVA, Jan 2020–Jan 2022.</li>
          <li><strong>Organizer</strong>, UVA CS Research Symposium, 2020 and 2021.</li>
          <li><strong>Social Chair</strong>, Association of Bangladeshi Students at UVA, Fall 2021–Summer 2022.</li>
          <li><strong>Recruiter</strong>, SWE24, Chicago, IL. Assisted UVA Engineering with recruiting, booth setup, and outreach.</li>
          <li><strong>Student Volunteer</strong>, ESEC/FSE 2023, San Francisco, CA. Assisted with registration, badge verification, presentation testing, A/V setup, and event preparation.</li>
          <li>Assisted UVA CS with faculty recruitment and graduate student visits.</li>
        </ul>
      </section>
    </div>
  </section>

  <section class="pi-section" id="teaching">
    <h2 class="pi-section-title">Teaching</h2>
    <div class="pi-grid">
      <section class="pi-card pi-span-12">
        <h3>CS/CE/SE 3354 — Software Engineering · Fall 2025</h3>
        <div class="pi-course-meta">
          <a href="https://catalog.utdallas.edu/2024/undergraduate/courses/cs3354">Catalog</a>
          <a href="https://assert-lab.github.io/teaching/CS3354_Fall2025_Syllabus.pdf">Syllabus</a>
          <span>UT Dallas</span>
        </div>
        <p><strong>Key Topics:</strong> Software processes, requirements engineering, UML modeling, design principles, testing, and team-based projects.</p>
        <div class="pi-course-grid">
          <div class="pi-mini-box">
            <h4>Course Learning Outcomes</h4>
            <ul>
              <li>Explain the software development lifecycle and its key phases.</li>
              <li>Apply software requirements engineering techniques to specify system behavior.</li>
              <li>Apply fundamental software design principles to create structured solutions.</li>
              <li>Apply software testing methods to ensure software quality.</li>
              <li>Integrate software engineering concepts through a collaborative, team-based project.</li>
            </ul>
          </div>
          <div class="pi-mini-box">
            <h4>Grading Breakdown</h4>
            <ul>
              <li>Deliverables (Team Project): 30%</li>
              <li>Assignments: 10%</li>
              <li>Midterm Exam: 25%</li>
              <li>Final Exam: 25%</li>
              <li>Participation & Attendance: 10%</li>
            </ul>
          </div>
        </div>
      </section>

      <section class="pi-card pi-span-6">
        <h3>CS/SE 6356 — Software Maintenance, Evolution & Re-engineering · Spring 2026</h3>
        <div class="pi-course-meta">
          <a href="https://catalog.utdallas.edu/2025/graduate/courses/cs6356">Catalog</a>
          <span>Cross-listed: SYSM 6308 / CS/SE 6356.001</span>
        </div>
        <p>
          Graduate course on software maintenance, evolution, and re-engineering.
        </p>
      </section>

      <section class="pi-card pi-span-6">
        <h3>Mentoring and Prior Teaching</h3>
        <ul>
          <li><strong>Faculty mentor</strong>, AS²ERT Lab undergraduate research projects through RIDE and URAP.</li>
          <li><strong>Graduate TA</strong>, CS 4620 Undergraduate Compilers and CS 6620 Graduate Compilers, UVA.</li>
          <li>Guest lectures in compilers and program analysis.</li>
          <li><strong>Undergraduate research mentor</strong>, more than 10 students from universities in the U.S. and Bangladesh.</li>
          <li><strong>Mentees included:</strong> Raygan Taylor, Javan Mendoza, Nicki Choquette, Kasra Lekan, Ashley Hart, Srikar Chittari, and Eric Weng.</li>
          <li><strong>BWCSE Mentor</strong>, Bangladeshi Women in Computer Science and Engineering; mentored BUET students preparing for research and graduate school.</li>
        </ul>
      </section>
    </div>
  </section>

  <section class="pi-archive-intro" id="phd-archive">
    <h2>Ph.D. Archive</h2>
    <p>
      Education, awards, service, and teaching are listed above once. This archive keeps the remaining graduate-school context and dated milestones from the earlier portfolio.
    </p>
  </section>

  <div class="pi-grid">
    <section class="pi-card pi-archive-card pi-span-12">
      <h3>Graduate-School Context</h3>
      <p>
        During my Ph.D., I collaborated with <strong>Lockheed Martin</strong> and <strong>AWS AI Labs</strong>. My graduate-school research focused on <strong>AI for Software Engineering</strong>, especially <em>requirements, testing, debugging, and repair</em> for software systems, with a long-term vision of advancing high-quality, reliable software through cost-effective automation powered by <strong>AI/ML</strong>, <strong>LLMs</strong>, and <strong>agentic AI</strong>.
      </p>
    </section>

    <section class="pi-card pi-archive-card pi-span-12">
      <h3>Archived Timeline</h3>
      <ul class="pi-timeline">
        <li><span class="pi-date">Aug 1, 2025</span><span>Joined CS@UTD as a tenure-track Assistant Professor.</span></li>
        <li><span class="pi-date">Jul 25, 2025</span><span>Relocated to Dallas, TX from Virginia.</span></li>
        <li><span class="pi-date">Jun 25, 2025</span><span>Attended FSE 2025 in Trondheim, Norway.</span></li>
        <li><span class="pi-date">Apr 25, 2025</span><span>Attended ICSE 2025 in Ottawa, Canada.</span></li>
        <li><span class="pi-date">Apr 25, 2025</span><span>Successfully defended my Ph.D. dissertation and officially became Dr. Soneya Binta Hossain.</span></li>
        <li><span class="pi-date">May 2024</span><span>Defended my Ph.D. dissertation proposal. <a href="{{ '/proposal/' | relative_url }}">[gallery]</a></span></li>
        <li><span class="pi-date">Apr 2024</span><span>Attended ICSE 2024 in Lisbon, Portugal, and participated in the Doctoral Symposium. <a href="{{ '/icse-24/' | relative_url }}">[gallery]</a></span></li>
        <li><span class="pi-date">Dec 2023</span><span>Attended FSE 2023 in San Francisco, CA. <a href="{{ '/FSE-23/' | relative_url }}">[gallery]</a></span></li>
        <li><span class="pi-date">May 2023</span><span>Attended ICSE 2023 in Melbourne, Australia. <a href="{{ '/ICSE-23/' | relative_url }}">[gallery]</a></span></li>
        <li><span class="pi-date">Apr 2023</span><span>Attended CRA Grad Cohort in San Francisco, CA. <a href="{{ '/CRA-SFO/' | relative_url }}">[gallery]</a></span></li>
        <li><span class="pi-date">Apr 2022</span><span>Attended ICSE 2022 in Pittsburgh, PA.</span></li>
        <li><span class="pi-date">Sep 2021</span><span>Passed the Ph.D. qualifying exam.</span></li>
        <li><span class="pi-date">Apr 2021</span><span>Attended the CRA-W Grad Cohort Workshop 2021 virtually.</span></li>
        <li><span class="pi-date">Aug 2019</span><span>Began Ph.D. in Computer Science at the University of Virginia.</span></li>
      </ul>
    </section>
  </div>

</div>
