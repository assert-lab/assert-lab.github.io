---
layout: default
permalink: /PI/
title: "Dr. Soneya Binta Hossain"
description: "Dr. Soneya Binta Hossain, Assistant Professor of Computer Science at The University of Texas at Dallas and Principal Investigator of the AS²ERT Lab."
---

<div class="wrap">
  <div class="pi-layout">

    <aside class="pi-aside">
      <img class="portrait" src="{{ '/assets/images/soneya.jpg' | relative_url }}" alt="Dr. Soneya Binta Hossain">
      <p class="aside-title">Assistant Professor<br>Department of Computer Science<br>The University of Texas at Dallas</p>

      <div class="aside-block">
        <h2>Links</h2>
        <ul>
          {% for link in site.author.links %}
          {% if link.url %}
          <li><a href="{{ link.url }}">{{ link.label }}</a></li>
          {% endif %}
          {% endfor %}
          <li><a href="{{ '/team/' | relative_url }}">AS²ERT Lab people</a></li>
        </ul>
      </div>

      <div class="aside-block toc-block">
        <h2>On this page</h2>
        <ul>
          <li><a href="#education">Education</a></li>
          <li><a href="#experience">Experience</a></li>
          <li><a href="#service">Service</a></li>
          <li><a href="#awards">Honors &amp; support</a></li>
          <li><a href="#teaching">Teaching &amp; mentoring</a></li>
          <li><a href="#timeline">Academic timeline</a></li>
        </ul>
      </div>
    </aside>

    <div class="pi-main">

      <div class="pi-intro" id="top">
        <p class="eyebrow">Principal Investigator, AS²ERT Lab</p>
        <h1>Dr. Soneya Binta Hossain</h1>
        <p class="role">Assistant Professor · Department of Computer Science · The University of Texas at Dallas</p>

        <p>I lead the AS²ERT Lab, AI for Safe Software Engineering and Testing, at UTD. My research focuses on verification and validation of both classical and quantum software systems. We aim to effectively combine AI with established software engineering techniques to improve software correctness checking and ensure reliability. A major part of my work also seeks to better understand the failure modes of AI-based development tools.</p>

        <p>My path to the AS²ERT Lab began at the Bangladesh University of Engineering and Technology (BUET), where I earned my B.Sc. in Computer Science and Engineering, and continued at the University of Virginia, where I earned my Ph.D. and M.S. in Computer Science under the guidance of <a href="https://matthewbdwyer.github.io">Prof. Matthew Dwyer</a>. During my Ph.D., I studied AI-driven approaches to automated software testing, work that now shapes the lab’s broader vision of building safer and more trustworthy software systems.</p>
      </div>

      <section class="cv-section" id="education">
        <h2>Education</h2>
        <ul class="cv">
          <li>
            <span class="cv-when">2025</span>
            <div><strong>Ph.D., Computer Science</strong>, University of Virginia. Dissertation: <em>Assessing and Improving Critical Properties of Test Oracles for Effective Software Bug Detection</em>.
              <span class="sub"><strong>Advisor:</strong> Matthew B. Dwyer. <strong>Committee Members:</strong> Sebastian Elbaum, Yangfeng Ji, Matthew Bolton, and Antonio Filieri.</span></div>
          </li>
          <li>
            <span class="cv-when">2024</span>
            <div><strong>M.C.S., Computer Science</strong>, University of Virginia. Project: <em>TOGLL: Correct and Strong Test Oracle Generation with Large Language Models</em>.</div>
          </li>
          <li>
            <span class="cv-when">2016</span>
            <div><strong>B.Sc., Computer Science and Engineering</strong>, Bangladesh University of Engineering and Technology. Thesis: <em>Balanced Coverage in Fault-Tolerant Broadcasting for Wireless Multi-hop Networks</em>.
              <span class="sub"><strong>Advisor:</strong> Dr. A.K.M. Ashikur Rahman.</span></div>
          </li>
        </ul>
      </section>

      <section class="cv-section" id="experience">
        <h2>Experience</h2>
        <ul class="cv">
          <li><span class="cv-when">2025–present</span><div><strong>Assistant Professor</strong>, Department of Computer Science, The University of Texas at Dallas.</div></li>
          <li><span class="cv-when">2019–2025</span><div><strong>Graduate Research and Teaching Assistant</strong>, Department of Computer Science, University of Virginia.</div></li>
          <li><span class="cv-when">2023</span><div><strong>Applied Scientist Intern</strong>, AWS CodeCatalyst.</div></li>
          <li><span class="cv-when">2022</span><div><strong>Applied Scientist Intern</strong>, AWS CodeGuru.</div></li>
          <li><span class="cv-when">2016–2019</span><div><strong>Software Development Engineer II</strong>, R&amp;D, REVE Systems.</div></li>
        </ul>
      </section>

      <section class="cv-section" id="service">
        <h2>Service</h2>

        <h3 class="subhead">External professional service</h3>
        <ul class="plain">
          <li><strong>Invited Panel Reviewer</strong>, National Science Foundation (NSF).</li>
          <li><strong>Program Committee Member</strong>, ACM International Conference on the Foundations of Software Engineering (FSE 2027), Research Papers track.</li>
          <li><strong>Program Committee Member</strong>, IEEE/ACM International Conference on Automated Software Engineering (ASE 2026), The New Ideas and Emerging Results (NIER) track.</li>
          <li><strong>Program Committee Member</strong>, IEEE/ACM International Conference on Automated Software Engineering (ASE 2026), Tools and Datasets track.</li>
          <li><strong>Program Committee Member</strong>, ACM International Conference on the Foundations of Software Engineering (FSE 2026), Ideas, Visions, and Reflections (IVR) track.</li>
          <li><strong>Program Committee Member</strong>, 3rd ACM International Conference on AI-Powered Software (AIware 2026).</li>
          <li><strong>Program Committee Member</strong>, IEEE International Conference on Software Testing, Verification and Validation (ICST 2025 and 2026).</li>
          <li><strong>Social Events Co-Chair</strong>, ACM SIGPLAN Conference on Systems, Programming, Languages, and Applications: Software for Humanity (SPLASH) / ACM SIGSOFT International Symposium on Software Testing and Analysis (ISSTA) 2026.</li>
          <li><strong>Reviewer</strong>, ACM Transactions on Software Engineering and Methodology (TOSEM).</li>
          <li><strong>Reviewer</strong>, <a href="https://link.springer.com/journal/10515">Automated Software Engineering</a> (Springer Nature).</li>
        </ul>

        <h3 class="subhead">Institutional and community service</h3>
        <ul class="plain">
          <li><strong>Ph.D. Admissions Committee</strong>, UTD CS, Fall 2025–present.</li>
          <li><strong>Course Coordinator</strong>, CS/CE/SE 3354 Software Engineering, UTD, Fall 2025–present.</li>
          <li><strong>Leadership Chair</strong>, UVA Computer Science Graduate Student Group, 2020–2022.</li>
          <li><strong>Student Volunteer:</strong> WE24/Society of Women Engineers and ESEC/FSE 2023.</li>
        </ul>
      </section>

      <section class="cv-section" id="awards">
        <h2>Honors, recognition, and research support</h2>

        <h3 class="subhead">Research awards</h3>
        <ul class="cv">
          <li><span class="cv-when">2023</span><div><strong>John A. Stankovic Outstanding Graduate Research Award</strong>, UVA <span class="note">(Ph.D.)</span>.</div></li>
          <li><span class="cv-when">2021, 2023</span><div><strong>Outstanding Research Award</strong>, UVA <span class="note">(Ph.D.)</span>.</div></li>
          <li><span class="cv-when">2016</span><div><strong>Outstanding Undergraduate Thesis Award</strong>, BUET <span class="note">(undergraduate)</span>.</div></li>
        </ul>

        <h3 class="subhead">Service awards</h3>
        <ul class="cv">
          <li><span class="cv-when">2026</span><div><strong>Grace Hopper Spirit Award</strong>, Department of Computer Science, UTD.</div></li>
          <li><span class="cv-when">2022</span><div><strong>Outstanding Graduate Service Award</strong>, UVA Computer Science <span class="note">(Ph.D.)</span>.</div></li>
        </ul>

        <h3 class="subhead">Fellowships and travel support</h3>
        <ul class="cv">
          <li><span class="cv-when">2024–2025</span><div><strong>UVA Endowed Ph.D. Fellowship</strong>, competitive fellowship.</div></li>
          <li><span class="cv-when">2025</span><div><strong>ACM SIGSOFT Travel Award</strong>.</div></li>
          <li><span class="cv-when">2014, 2020, 2023</span><div><strong>CRA Travel Grants</strong>.</div></li>
        </ul>

        <h3 class="subhead">Research group support at UTD</h3>
        <ul class="cv">
          <li><span class="cv-when">2026</span><div><strong>Presidential Fellowship</strong> for one Ph.D. student, UTD, $37,000.</div></li>
          <li><span class="cv-when"></span><div><strong>UTD Undergraduate Research Support</strong>, $10,500.</div></li>
        </ul>
      </section>

      <section class="cv-section" id="teaching">
        <h2>Teaching and mentoring</h2>

        <h3 class="subhead">Teaching at UTD</h3>
        <ul class="plain">
          <li><strong>CS/SE/SYSM 6356:</strong> Software Maintenance, Evolution &amp; Re-engineering, UTD.</li>
          <li><strong>CS/CE/SE 3354:</strong> Software Engineering, UTD.</li>
        </ul>

        <h3 class="subhead">Mentoring</h3>
        <ul class="plain">
          <li>Research mentor for high school, undergraduate, M.S., and Ph.D. students across multiple institutions.</li>
          <li><strong>RIDE:</strong> Research, Inquiry, Design Experience, UTD undergraduate research program.</li>
        </ul>

        <h3 class="subhead">Prior teaching experience (Ph.D.)</h3>
        <ul class="plain">
          <li><strong>Graduate TA:</strong> CS 4620 Undergraduate Compilers and CS 6620 Graduate Compilers, UVA.</li>
        </ul>
      </section>

      <section class="cv-section" id="timeline">
        <h2>Academic timeline</h2>
        <ul class="cv">
          <li><span class="cv-when">Aug 2025</span><div>Joined CS@UTD as a tenure-track Assistant Professor.</div></li>
          <li><span class="cv-when">Jun 2025</span><div>Attended FSE 2025 in Trondheim, Norway, and presented our paper.</div></li>
          <li><span class="cv-when">Apr 2025</span><div>Defended my Ph.D. dissertation and attended ICSE 2025 in Ottawa, Canada, where I presented our paper.</div></li>
          <li><span class="cv-when">May 2024</span><div>Defended my Ph.D. dissertation proposal. <a class="more" href="{{ '/proposal/' | relative_url }}">Gallery →</a></div></li>
          <li><span class="cv-when">Apr 2024</span><div>Attended ICSE 2024 in Lisbon, Portugal, participated in the Doctoral Symposium, and presented my paper. <a class="more" href="{{ '/icse-24/' | relative_url }}">Gallery →</a></div></li>
          <li><span class="cv-when">Dec 2023</span><div>Attended FSE 2023 in San Francisco, CA, and presented our paper. <a class="more" href="{{ '/FSE-23/' | relative_url }}">Gallery →</a></div></li>
          <li><span class="cv-when">May 2023</span><div>Attended ICSE 2023 in Melbourne, Australia, and presented our paper. <a class="more" href="{{ '/ICSE-23/' | relative_url }}">Gallery →</a></div></li>
          <li><span class="cv-when">Sep 2021</span><div>Passed the Ph.D. qualifying exam.</div></li>
          <li><span class="cv-when">Aug 2019</span><div>Began my Ph.D. in Computer Science at the University of Virginia.</div></li>
        </ul>
      </section>

    </div>
  </div>
</div>
