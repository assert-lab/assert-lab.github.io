---
layout: page
title: "Focus Research Areas"
permalink: /research/
classes: wide
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

<p style="font-size:0.98em; line-height:1.6;">
  My research lies at the intersection of <strong>program analysis</strong> and <strong>artificial intelligence</strong>, 
  focusing on advancing software quality, reliability, and automation through data-driven and learning-based approaches.
  Below are my key research areas that guide the ongoing and future directions of my lab.
</p>

<div class="research-grid">

  <section class="research-card">
    <h3>1️⃣ AI for Software Reliability</h3>
    <p>
      This area explores how artificial intelligence can support the creation of dependable software systems.
      We examine learning-based methods that analyze programs, reason about behavior, and assist developers in improving quality and maintainability.
    </p>
  </section>

  <section class="research-card">
    <h3>2️⃣ Intelligent Testing and Validation</h3>
    <p>
      Software testing remains central to ensuring correctness. 
      This area focuses on designing intelligent, data-driven techniques for test design and validation,
      leveraging knowledge from code, documentation, and prior executions to improve automation and reduce cost.
    </p>
  </section>

  <section class="research-card">
    <h3>3️⃣ Trustworthy and Emerging Computing</h3>
    <p>
      As computing expands into new paradigms, such as quantum and hybrid systems,
      ensuring reliability becomes increasingly complex. 
      This area investigates how automated reasoning and AI-driven analysis can enhance assurance and testing for such emerging domains.
    </p>
  </section>

</div>

---

<p style="text-align:center; font-size:0.95em; color:#666;">
  🧠 For publications and recent work, visit the 
  <a href="/publications/" style="color:#ff6600; font-weight:600;">Publications</a> and 
  <a href="/news/" style="color:#ff6600; font-weight:600;">Lab News</a> pages.
</p>
