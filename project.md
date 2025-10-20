---
layout: single
title: "Focus Research Areas"
permalink: /project/
classes: wide
author_profile: true
---

<style>
  .research-grid {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    gap: 18px;
  }
  @media (max-width:1024px){ .research-grid{ grid-template-columns: repeat(6,1fr);} }
  @media (max-width:640px){ .research-grid{ grid-template-columns: repeat(2,1fr);} }

  .research-card {
    grid-column: span 6;
    background: #fff;
    border: 2px solid #ff6600;
    border-radius: 14px;
    padding: 18px;
    box-shadow: 0 6px 18px rgba(0,0,0,0.06);
  }
  .research-card h3 {
    margin-top: 0;
    color: #ff6600;
    font-size: 1.15rem;
  }
  .research-card p {
    margin-top: 8px;
    font-size: 0.95em;
    line-height: 1.55;
  }
</style>


<div class="research-grid">

  <section class="research-card">
    <h3>1️⃣ Robust and Trustworthy AI for Software Engineering</h3>
    <p>
      We study how large language models (LLMs) and AI-based tools can be made more resilient, consistent, 
      and trustworthy when reasoning about source code. 
      This includes understanding how AI systems respond to imperfect or buggy code and designing strategies 
      that improve their reliability in practical software development contexts.
    </p>
  </section>

  <section class="research-card">
    <h3>2️⃣ Automated Quality Assurance and Test Intelligence</h3>
    <p>
      This area focuses on advancing automation in software testing—particularly in how systems learn to identify 
      correct versus incorrect program behaviors. 
      We investigate intelligent agents that can reason about program outputs, 
      supported by high-quality datasets and evaluation frameworks that reflect real-world testing practices.
    </p>
  </section>

  <section class="research-card">
    <h3>3️⃣ Data-Centric Foundations for Reliable Testing</h3>
    <p>
      High-quality datasets are critical to developing effective AI for testing and validation. 
      Our research examines how to curate, synthesize, and structure test data derived from human-written tests 
      and other software artifacts, enabling systematic exploration of correctness and coverage in diverse settings.
    </p>
  </section>

  <section class="research-card">
    <h3>4️⃣ Cross-Domain Software Assurance</h3>
    <p>
      Emerging computing paradigms—such as quantum and hybrid software—pose new challenges for testing and analysis. 
      We explore how classical software engineering principles can enhance the testing of quantum systems, 
      and conversely, how quantum-inspired methods can inform next-generation testing strategies for traditional software.
    </p>
  </section>

</div>

---

<p style="text-align:center; font-size:0.95em; color:#666;">
  🧠 For publications and recent work, visit the 
  <a href="/publications/" style="color:#ff6600; font-weight:600;">Publications</a> and 
  <a href="/news/" style="color:#ff6600; font-weight:600;">Lab News</a> pages.
</p>
