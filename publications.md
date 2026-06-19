---
layout: single
title: "Publications"
permalink: /publications/
classes: wide publications
author_profile: true
---

<style>
/* ===============================
   Publications page (scoped, homepage theme)
   Fix: icons use a grid column instead of absolute positioning,
   so they cannot overlap titles or author text.
   =============================== */
.pub-header,
.pub-section,
.pub-footer {
  --utd-green: #154734;
  --utd-orange: #E87500;
  --pub-text: #1f2937;
  --pub-muted: #6b7280;
  --pub-border: rgba(21, 71, 52, 0.18);
  --pub-shadow: 0 10px 22px rgba(0,0,0,0.05);
}

.pub-header {
  background: linear-gradient(135deg, rgba(21,71,52,0.10), rgba(232,117,0,0.12));
  border: 1px solid rgba(0,0,0,0.06);
  border-radius: 18px;
  padding: 20px 22px;
  box-shadow: 0 12px 28px rgba(0,0,0,0.06);
  margin-bottom: 18px;
  color: var(--pub-text);
  line-height: 1.7;
}

.pub-header a,
.pub-footer a,
.pub-links a {
  color: var(--utd-orange);
  text-decoration: none;
  font-weight: 700;
}

.pub-header a:hover,
.pub-footer a:hover,
.pub-links a:hover {
  text-decoration: underline;
}

.pub-section {
  background: #ffffff;
  border: 1px solid rgba(0,0,0,0.07);
  border-radius: 16px;
  padding: 20px 20px 18px;
  box-shadow: var(--pub-shadow);
  margin-bottom: 18px;
}

.pub-section h3 {
  margin: 0 0 14px 0;
  color: var(--utd-green);
  font-size: 1.35rem;
  line-height: 1.25;
  letter-spacing: -0.01em;
}

.pub-entry {
  position: relative;
  display: grid;
  grid-template-columns: 34px minmax(0, 1fr);
  column-gap: 12px;
  align-items: start;
  margin: 14px 0;
  padding: 16px 16px 14px 16px;
  border: 1px solid var(--pub-border);
  border-radius: 14px;
  background:
    linear-gradient(135deg, rgba(21, 71, 52, 0.045), rgba(232, 117, 0, 0.035)),
    #ffffff;
  color: var(--pub-text);
  line-height: 1.65;
  box-shadow: 0 6px 16px rgba(0,0,0,0.035);
  overflow: hidden;
}

.pub-entry:first-of-type {
  margin-top: 0;
}

.pub-entry:last-of-type {
  margin-bottom: 0;
}

.pub-entry::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  width: 4px;
  border-radius: 14px 0 0 14px;
  background: linear-gradient(180deg, var(--utd-green), var(--utd-orange));
}

.pub-icon {
  position: relative;
  z-index: 1;
  width: 30px;
  height: 30px;
  margin-top: 2px;
  border-radius: 999px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  flex: 0 0 30px;
  color: var(--utd-green);
  background: rgba(21, 71, 52, 0.08);
  border: 1px solid rgba(21, 71, 52, 0.16);
  line-height: 1;
}

.pub-icon i {
  display: block;
  font-size: 0.92rem;
  line-height: 1;
}

.pub-content {
  position: relative;
  z-index: 1;
  min-width: 0;
  overflow-wrap: break-word;
}

.pub-title {
  display: block;
  color: var(--pub-text);
  font-size: 1.03rem;
  line-height: 1.4;
  margin-bottom: 2px;
}

.pub-entry em {
  color: var(--utd-green);
  font-style: normal;
  font-weight: 800;
}

.pub-entry span {
  color: #374151;
}

.pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 8px;
}

.pub-links a {
  display: inline-flex;
  align-items: center;
  border: 1px solid rgba(21, 71, 52, 0.18);
  border-radius: 999px;
  padding: 3px 9px;
  background: #f3f4f6;
  color: var(--utd-green);
  font-size: 0.78rem;
  font-weight: 700;
}

.pub-links a:hover {
  background: var(--utd-green);
  color: #ffffff;
  border-color: var(--utd-green);
  text-decoration: none;
}

.pub-footer {
  border-left: 5px solid var(--utd-orange);
  background: rgba(232,117,0,0.10);
  border-radius: 14px;
  padding: 14px 16px;
  margin: 18px 0 0 0;
  line-height: 1.7;
}

.publications .page__content hr {
  border: 0;
  height: 1px;
  background: linear-gradient(90deg, transparent, rgba(21, 71, 52, 0.18), transparent);
  margin: 18px 0;
}

@media (max-width: 640px) {
  .pub-header,
  .pub-section {
    padding: 18px 16px 16px;
  }

  .pub-entry {
    grid-template-columns: 30px minmax(0, 1fr);
    column-gap: 10px;
    padding: 15px 14px 13px 14px;
  }

  .pub-icon {
    width: 28px;
    height: 28px;
    flex-basis: 28px;
  }
}
</style>

---

<div class="pub-header">
  📚 A full list of publications is available on
  <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&hl=en">Google Scholar</a>.
</div>

<div class="pub-section">
  <h3>Publications (Peer-reviewed)</h3>


   <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">PITMuS: A Tool for Automated Bug Dataset Generation via Source-Level Mutant Reconstruction</strong>
      Tasfia Tasnim, <em>Soneya Binta Hossain</em> <br>
      <span>IEEE/ACM International Conference on Automated Software Engineering (<strong> ASE 2026, Tools & Datasets Track </strong>)</span><br>
      <div class="pub-links">
        <a href="https://github.com/assert-lab/OE25-DEV">[GitHub]</a>
      </div>
    </div>
  </div>

  <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">TOGBench: A Developer-Written Multi-Variant Dataset and Benchmark Suite for Test Oracle Generation</strong>
      Tasfia Tasnim, Matthew Dwyer, <em>Soneya Binta Hossain</em> <br>
      <span>3rd ACM International Conference on AI-Powered Software (<strong>AIware 2026 Benchmark & Dataset Track</strong>)</span><br>
      <div class="pub-links">
        <a href="https://github.com/assert-lab/OE25-DEV">[GitHub]</a>
      </div>
    </div>
  </div>

  <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">Doc2OracLL: Investigating the Impact of Documentation on LLM-based Test Oracle Generation</strong>
      <em>Soneya Binta Hossain</em>, Raygan Taylor, Matthew Dwyer<br>
      <span>The ACM International Conference on the Foundations of Software Engineering (<strong>FSE 2025</strong>)</span><br>
      <div class="pub-links">
        <a href="https://dl.acm.org/doi/abs/10.1145/3729354">[Paper]</a>
      </div>
    </div>
  </div>

  <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">TOGLL: Correct and Strong Test Oracle Generation with LLMs</strong>
      <em>Soneya Binta Hossain</em>, Matthew Dwyer<br>
      <span>The 47th International Conference on Software Engineering (<strong>ICSE 2025</strong>)</span><br>
      <div class="pub-links">
        <a href="https://ieeexplore.ieee.org/abstract/document/11029748">[Paper]</a>
        <a href="https://doi.org/10.6084/m9.figshare.28282721">[Artifact]</a>
      </div>
    </div>
  </div>

  <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">A Deep Dive into Large Language Models for Automated Bug Localization and Repair</strong>
      <em>Soneya Binta Hossain</em>, Nan Jiang, Qiang Zhou, Xiaopeng Li, Wen-Hao Chiang, Yingjun Lyu, Hoan Nguyen, Omer Tripp<br>
      <span>ACM International Conference on the Foundations of Software Engineering (<strong>FSE 2024</strong>)</span><br>
      <div class="pub-links">
        <a href="https://dl.acm.org/doi/abs/10.1145/3660773">[Paper]</a>
        <a href="https://www.amazon.science/publications/a-deep-dive-into-large-language-models-for-automated-bug-localization-and-repair">[Amazon Science Blog]</a>
      </div>
    </div>
  </div>

  <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">Ensuring Critical Properties of Test Oracles for Effective Bug Detection</strong>
      <em>Soneya Binta Hossain</em><br>
      <span>The 46th International Conference on Software Engineering (<strong>ICSE Doctoral Symposium 2024</strong>)</span><br>
      <div class="pub-links">
        <a href="https://dl.acm.org/doi/10.1145/3639478.3639791">[Paper]</a>
        <a href="/assets/presentations/ICSE-DS-24-Soneya-A0-28.pdf">[Poster]</a>
      </div>
    </div>
  </div>

  <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">LEDEX: Training LLMs to Better Self-Debug and Explain Code</strong>
      Nan Jiang, Xiaopeng Li, Shiqi Wang, Qiang Zhou, <em>Soneya Binta Hossain</em>, Baishakhi Ray, Varun Kumar, Xiaofei Ma<br>
      <span>The 38th Conference on Neural Information Processing Systems (<strong>NeurIPS 2024</strong>)</span> [Acceptance Rate: 25%]<br>
      <div class="pub-links">
        <a href="https://dl.acm.org/doi/10.5555/3737916.3739036">[Paper]</a>
        <a href="https://www.amazon.science/blog/training-code-generation-models-to-debug-their-own-outputs">[Amazon Science Blog]</a>
      </div>
    </div>
  </div>

  <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">Measuring and Mitigating Gaps in Structural Testing</strong>
      <em>Soneya Binta Hossain</em>, Matthew Dwyer, Sebastian Elbaum, Anh Nguyen-Tuong<br>
      <span>The 45th International Conference on Software Engineering (<strong>ICSE 2023</strong>)</span> [Acceptance Rate: 26%]<br>
      <div class="pub-links">
        <a href="https://ieeexplore.ieee.org/abstract/document/10172745">[Paper]</a>
        <a href="https://github.com/soneyahossain/hcc-gap-recommender/tree/main">[Artifact]</a>
      </div>
    </div>
  </div>

  <div class="pub-entry">
    <span class="pub-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <div class="pub-content">
      <strong class="pub-title">Neural-Based Test Oracle Generation: A Large-Scale Evaluation and Lessons Learned</strong>
      <em>Soneya Binta Hossain</em>, Antonio Filieri, Matthew Dwyer, Sebastian Elbaum, Willem Visser<br>
      <span>The 31st ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (<strong>ESEC/FSE 2023</strong>)</span> [Acceptance Rate: 21%]<br>
      <div class="pub-links">
        <a href="https://dl.acm.org/doi/abs/10.1145/3611643.3616265">[Paper]</a>
        <a href="https://doi.org/10.6084/m9.figshare.21973091.v4">[Artifact]</a>
      </div>
    </div>
  </div>
</div>

<hr>

<p class="pub-footer">
  🔍 For the complete list of publications, please visit my
  <a href="https://scholar.google.com/citations?user=xDDfwB8AAAAJ&hl=en">Google Scholar</a> profile.
</p>
