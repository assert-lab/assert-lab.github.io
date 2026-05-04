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
    line-height:1.62;
  }

  .pi-page a{
    color:var(--pi-orange);
    text-decoration:none;
    font-weight:700;
  }

  .pi-page a:hover{ text-decoration:underline; }

  .pi-hero{
    border:1px solid var(--pi-line);
    border-radius:24px;
    padding:30px 32px;
    margin-bottom:22px;
    background:
      radial-gradient(circle at 92% 8%, rgba(199,91,18,.15), transparent 34%),
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

  .pi-section{ margin:24px 0; }

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
    padding:19px 20px 17px 22px;
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
.pi-span-12 {
  grid-column: span 12;
}
  .pi-card h3{
    margin:0 0 9px 0;
    font-weight:850;
    line-height:1.25;
    letter-spacing:-.01em;
    font-size:1.08rem;
  }

  .pi-card p{ margin:0 0 10px 0; }
  .pi-card p:last-child{ margin-bottom:0; }
  .pi-card ul{ margin:8px 0 0 20px; }
  .pi-card li{ margin:6px 0; }

  .pi-span-12{ grid-column:span 12; }
  .pi-span-6{ grid-column:span 6; }

  .pi-compact-list li{ margin:5px 0; }

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
    grid-template-columns:110px 1fr;
    gap:10px;
    margin:8px 0;
    padding:0 0 8px 0;
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
    .pi-span-12,.pi-span-6,.pi-card{ grid-column:span 6; }
  }

  @media (max-width:640px){
    .pi-hero{ padding:22px 20px; }
    .pi-hero h1{ font-size:1.82rem; }
    .pi-grid{ grid-template-columns:repeat(2,1fr); }
    .pi-span-12,.pi-span-6,.pi-card{ grid-column:span 2; }
    .pi-timeline li{ grid-template-columns:1fr; gap:2px; }
  }
</style>

<div class="pi-page">

  <section class="pi-hero" id="top">
    <p class="pi-kicker">Principal Investigator, AS²ERT Lab</p>
    <h1>Dr. Soneya Binta Hossain</h1>
    <p class="pi-title">Assistant Professor · Department of Computer Science · The University of Texas at Dallas</p>

    <p class="pi-summary">
      I lead the AS²ERT Lab — AI for Safe Software Engineering and Testing — at UTD. My research focuses on verification and validation of both classical and quantum software systems. We aim to effectively combine AI with established software engineering techniques to improve software correctness checking and ensure reliability. A major part of my work also seeks to better understand the failure modes of AI-based development tools.  
      

My path to the AS²ERT Lab began at the Bangladesh University of Engineering and Technology (BUET), where I earned my B.Sc. in Computer Science and Engineering, and continued at the University of Virginia, where I earned my Ph.D. and M.S. in Computer Science under the guidance of <a href="https://matthewbdwyer.github.io">Prof. Matthew Dwyer</a>. During my Ph.D., I studied AI-driven approaches to automated software testing — work that now shapes the lab’s broader vision of building safer and more trustworthy software systems.
    </p>

    <div class="pi-actions">
      <a class="pi-button primary" href="#education">Education</a>
      <a class="pi-button primary" href="#experience">Experience</a>
      <a class="pi-button" href="#service">Service</a>
      <a class="pi-button" href="#awards">Awards</a>
      <a class="pi-button" href="#grants">Grants</a>
      <a class="pi-button" href="#teaching">Teaching</a>
      <a class="pi-button" href="#phd-archive">Ph.D. Archive</a>
    </div>
  </section>


 
         <section class="pi-section" id="education">
    <h2 class="pi-section-title">Education</h2>
    <div class="pi-grid">
      <section class="pi-card pi-span-12">
        <ul class="pi-compact-list">
          <li><strong>Ph.D., Computer Science</strong>, University of Virginia, 2025. Dissertation: <em>Assessing and Improving Critical Properties of Test Oracles for Effective Software Bug Detection</em>.<br>
            <strong>Advisor:</strong> Matthew B. Dwyer. <strong>Committee Members:</strong> Sebastian Elbaum, Yangfeng Ji, Matthew Bolton, and Antonio Filieri.</li>
          <li><strong>M.C.S., Computer Science</strong>, University of Virginia, 2024. Project: <em>TOGLL: Correct and Strong Test Oracle Generation with Large Language Models</em>.</li>
          <li><strong>B.Sc., Computer Science and Engineering</strong>, Bangladesh University of Engineering and Technology, 2016. Thesis: <em>Balanced Coverage in Fault-Tolerant Broadcasting for Wireless Multi-hop Networks</em>.<br>
          <strong>Advisor:</strong> Dr. A.K.M. Ashikur Rahman.</li>
        </ul>
      </section>
    </div>
  </section>
          

  <section class="pi-section" id="experience">
    <h2 class="pi-section-title">Experience</h2>
    <div class="pi-grid">
      <section class="pi-card pi-span-12">
        <ul class="pi-compact-list">
          <li><strong>Assistant Professor</strong>, Department of Computer Science, The University of Texas at Dallas, 2025–present.</li>
          <li><strong>Graduate Research and Teaching Assistant</strong>, Department of Computer Science, University of Virginia, 2019–2025.</li>
          <li><strong>Applied Scientist Intern</strong>, AWS CodeCatalyst, 2023.</li>
          <li><strong>Applied Scientist Intern</strong>, AWS CodeGuru, 2022.</li>
          <li><strong>Software Development Engineer II </strong>, R&amp;D, REVE Systems, 2016–2019.</li>
        </ul>
      </section>
    </div>
  </section>
<section class="pi-section" id="service">
  <h2 class="pi-section-title">Service</h2>
  <div class="pi-grid">
    <section class="pi-card pi-span-12">
      <h3>External Professional Service</h3>
      <ul class="pi-compact-list">
        <li><strong>Invited Panel Reviewer</strong>, National Science Foundation (NSF).</li>
        <li><strong>Program Committee Member</strong>, ACM International Conference on the Foundations of Software Engineering (FSE 2027), Research Papers track.</li>
        <li><strong>Program Committee Member</strong>, IEEE/ACM International Conference on Automated Software Engineering (ASE 2026), The New Ideas and Emerging Results (NIER) track.</li>
        <li><strong>Program Committee Member</strong>, IEEE/ACM International Conference on Automated Software Engineering (ASE 2026), Tools and Datasets track.</li>
        <li><strong>Program Committee Member</strong>, ACM International Conference on the Foundations of Software Engineering (FSE 2026), Ideas, Visions, and Reflections (IVR) track.</li>
        <li><strong>Program Committee Member</strong>, 3rd ACM International Conference on AI-Powered Software (AIware 2026).</li>
        <li><strong>Program Committee Member</strong>, IEEE International Conference on Software Testing, Verification and Validation (ICST 2025 and 2026).</li>
        <li><strong>Social Events Co-Chair</strong>, ACM SIGPLAN Conference on Systems, Programming, Languages, and Applications: Software for Humanity (SPLASH) / ACM SIGSOFT International Symposium on Software Testing and Analysis (ISSTA) 2026.</li>
        <li><strong>Reviewer</strong>, ACM Transactions on Software Engineering and Methodology (TOSEM).</li>
      </ul>
    </section>

    <section class="pi-card pi-span-12">
      <h3>Institutional and Community Service</h3>
      <ul class="pi-compact-list">
        <li><strong>Ph.D. Admissions Committee</strong>, UTD CS, Fall 2025–present.</li>
        <li><strong>Course Coordinator</strong>, CS/CE/SE 3354 Software Engineering, UTD, Fall 2025–present.</li>
        <li><strong>Leadership Chair</strong>, UVA Computer Science Graduate Student Group, 2020–2022.</li>
        <li><strong>Student Volunteer:</strong> WE24/Society of Women Engineers and ESEC/FSE 2023.</li>
      </ul>
    </section>
  </div>
</section>








 




<section class="pi-section" id="awards">
  <h2 class="pi-section-title">Honors, Recognition, and Research Support</h2>
  <div class="pi-grid">
    <section class="pi-card pi-span-12">

      <h3>Research Awards</h3>
      <ul class="pi-compact-list">
        <li><strong>John A. Stankovic Outstanding Graduate Research Award</strong>, UVA, 2023 <span class="pi-note">(Ph.D.)</span>.</li>
        <li><strong>Outstanding Research Award</strong>, UVA, 2021 and 2023 <span class="pi-note">(Ph.D.)</span>.</li>
        <li><strong>Outstanding Undergraduate Thesis Award</strong>, BUET, 2016 <span class="pi-note">(undergraduate)</span>.</li>
      </ul>

      <h3>Service Awards</h3>
      <ul class="pi-compact-list">
        <li><strong>Grace Hopper Spirit Award</strong>, Department of Computer Science, UTD, 2026.</li>
        <li><strong>Outstanding Graduate Service Award</strong>, UVA Computer Science, 2022 <span class="pi-note">(Ph.D.)</span>.</li>
      </ul>

      <h3>Fellowships and Travel Support</h3>
      <ul class="pi-compact-list">
        <li><strong>UVA Endowed Ph.D. Fellowship</strong>, competitive fellowship, 2024-2025.</li>
        <li><strong>ACM SIGSOFT Travel Award</strong>, 2025.</li>
        <li><strong>CRA Travel Grants</strong>, 2014, 2020 and 2023.</li>
      </ul>

      <h3>Research Group Support at UTD</h3>
      <ul class="pi-compact-list">
        <li><strong>Presidential Fellowship</strong> for one Ph.D. student, UTD, 2026, $37,000.</li>
        <li><strong>UTD Undergraduate Research Support</strong> $10,500.</li>
      </ul>
    </section>
  </div>
</section>



<section class="pi-section" id="teaching">
  <h2 class="pi-section-title">Teaching and Mentoring</h2>
  <div class="pi-grid">
    <section class="pi-card pi-span-12">

      <h3>Teaching at UTD</h3>
      <ul class="pi-compact-list">
        <li><strong>CS/SE/SYSM 6356:</strong> Software Maintenance, Evolution &amp; Re-engineering, UTD.</li>
        <li><strong>CS/CE/SE 3354:</strong> Software Engineering, UTD.</li>
        <li><strong>RIDE:</strong> Research, Inquiry, Design Experience, UTD undergraduate research program.</li>
      </ul>

      <h3>Prior Experience (Ph.D.)</h3>
      <ul class="pi-compact-list">
        <li><strong>Graduate TA:</strong> CS 4620 Undergraduate Compilers and CS 6620 Graduate Compilers, UVA.</li>
        <li>Research mentor for high school, undergraduate, M.S., and Ph.D. students across multiple institutions.</li>
      </ul>

    </section>
  </div>
</section>

  
<div class="pi-grid">
  <section class="pi-card pi-archive-card pi-span-12">
    <h3>Academic Timeline</h3>
    <ul class="pi-timeline">
      <li><span class="pi-date">Aug 2025</span><span>Joined CS@UTD as a tenure-track Assistant Professor.</span></li>
      <li><span class="pi-date">Jun 2025</span><span>Attended FSE 2025 in Trondheim, Norway, and presented our paper.</span></li>
      <li><span class="pi-date">Apr 2025</span><span>Defended my Ph.D. dissertation and attended ICSE 2025 in Ottawa, Canada, where I presented our paper.</span></li>
      <li><span class="pi-date">May 2024</span><span>Defended my Ph.D. dissertation proposal. <a href="{{ '/proposal/' | relative_url }}">[gallery]</a></span></li>
      <li><span class="pi-date">Apr 2024</span><span>Attended ICSE 2024 in Lisbon, Portugal, participated in the Doctoral Symposium, and presented my paper. <a href="{{ '/icse-24/' | relative_url }}">[gallery]</a></span></li>
      <li><span class="pi-date">Dec 2023</span><span>Attended FSE 2023 in San Francisco, CA, and presented our paper. <a href="{{ '/FSE-23/' | relative_url }}">[gallery]</a></span></li>
      <li><span class="pi-date">May 2023</span><span>Attended ICSE 2023 in Melbourne, Australia, and presented our paper. <a href="{{ '/ICSE-23/' | relative_url }}">[gallery]</a></span></li>
      <li><span class="pi-date">Sep 2021</span><span>Passed the Ph.D. qualifying exam.</span></li>
      <li><span class="pi-date">Aug 2019</span><span>Began my Ph.D. in Computer Science at the University of Virginia.</span></li>
    </ul>
  </section>
</div>

</div>
