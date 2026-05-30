---
layout: single
title: ""
permalink: /team/
classes: wide
toc: false
---

<style>
/* ===============================
   Team page (scoped)
   Matches AS²ERT Lab homepage theme
   =============================== */
.team-page {
  --utd-green: #154734;
  --utd-orange: #E87500;
  --team-text: #1f2937;
  --team-muted: #6b7280;
  --team-border: rgba(21, 71, 52, 0.18);
  --team-soft: rgba(21, 71, 52, 0.06);
  --team-orange-soft: rgba(232, 117, 0, 0.10);
  --team-shadow: 0 10px 22px rgba(0,0,0,0.05);
  color: var(--team-text);
  font: inherit;
  font-size: 0.98rem;
  line-height: 1.65;
}

.team-page a {
  color: var(--utd-orange);
  text-decoration: none;
  font-weight: 700;
}

.team-page a:hover {
  text-decoration: underline;
}

.team-hero {
  background: linear-gradient(135deg, rgba(21,71,52,0.10), rgba(232,117,0,0.12));
  border: 1px solid rgba(0,0,0,0.06);
  border-radius: 18px;
  padding: 28px;
  box-shadow: 0 12px 28px rgba(0,0,0,0.06);
  margin-bottom: 18px;
}

.team-hero-inner {
  display: grid;
  grid-template-columns: 190px minmax(0, 1fr);
  gap: 24px;
  align-items: center;
}

.team-pi-photo {
  width: 180px;
  max-width: 100%;
  border-radius: 16px;
  border: 4px solid #ffffff;
  box-shadow: 0 12px 24px rgba(0,0,0,0.10);
}

.team-kicker {
  margin: 0 0 6px 0;
  color: var(--utd-green);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-size: 0.78rem;
  font-weight: 900;
}

.team-hero h1 {
  margin: 0 0 8px 0;
  font-size: 2rem;
  line-height: 1.15;
  color: var(--team-text);
}

.team-titleline {
  margin: 0;
  line-height: 1.65;
  max-width: 80ch;
}

.team-link-row {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 14px;
}

.team-button {
  display: inline-flex;
  align-items: center;
  gap: 7px;
  padding: 6px 11px;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid rgba(21, 71, 52, 0.24);
  color: var(--utd-green) !important;
  font-size: 0.9rem;
  font-weight: 800;
  text-decoration: none !important;
}

.team-button:hover {
  background: var(--utd-green);
  color: #ffffff !important;
}

.team-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 16px;
  align-items: start;
}

.team-card {
  grid-column: span 12;
  background: #ffffff;
  border: 1px solid rgba(0,0,0,0.07);
  border-radius: 16px;
  padding: 18px;
  box-shadow: var(--team-shadow);
  position: relative;
  overflow: hidden;
}

.team-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  width: 5px;
  background: linear-gradient(180deg, var(--utd-green), rgba(232,117,0,0.55));
}

.team-card.team-half {
  grid-column: span 6;
}

.team-card.team-full {
  grid-column: span 12;
}

.team-card h2 {
  margin: 0 0 12px 0;
  padding-left: 10px;
  font-size: 1.35rem;
  line-height: 1.25;
  color: var(--utd-green);
}

.team-card h3 {
  margin: 0 0 12px 0;
  font-size: 1.08rem;
  color: var(--utd-green);
}

.member-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  gap: 14px;
  padding-left: 10px;
}

.member-card {
  min-height: 100%;
  border: 1px solid var(--team-border);
  border-radius: 14px;
  background: linear-gradient(180deg, #ffffff, rgba(21,71,52,0.025));
  padding: 16px;
  text-align: center;
}

.member-card.with-photo {
  padding-top: 18px;
}

.member-card img {
  width: 142px;
  height: 142px;
  object-fit: cover;
  border-radius: 14px;
  margin-bottom: 10px;
  border: 3px solid #ffffff;
  box-shadow: 0 9px 18px rgba(0,0,0,0.10);
}

.member-placeholder {
  width: 58px;
  height: 58px;
  border-radius: 50%;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 10px;
  background: var(--team-soft);
  color: var(--utd-green);
  border: 1px solid var(--team-border);
  font-weight: 900;
  font-size: 1.35rem;
}

.member-name {
  display: block;
  margin-bottom: 4px;
  color: var(--team-text);
  font-size: 1.05rem;
}

.member-role {
  color: var(--team-muted);
  font-size: 0.94rem;
  line-height: 1.45;
}

.member-links {
  margin-top: 9px;
  font-size: 0.9rem;
}

.undergrad-wrapper {
  display: grid;
  grid-template-columns: 1fr;
  gap: 14px;
  padding-left: 10px;
}

.semester-card {
  border: 1px solid var(--team-border);
  border-left: 5px solid var(--utd-orange);
  border-radius: 14px;
  padding: 15px;
  background: linear-gradient(135deg, rgba(21,71,52,0.045), rgba(232,117,0,0.055));
}

.name-chip-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(165px, 1fr));
  gap: 8px;
}

.name-chip {
  display: flex;
  align-items: center;
  min-height: 34px;
  padding: 6px 9px;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid rgba(21, 71, 52, 0.18);
  color: var(--team-text);
  font-size: 0.88rem;
  line-height: 1.25;
  box-shadow: 0 4px 10px rgba(0,0,0,0.025);
}

.name-chip::before {
  content: "";
  width: 6px;
  height: 6px;
  flex: 0 0 6px;
  border-radius: 50%;
  margin-right: 7px;
  background: var(--utd-orange);
}

.alumni-card {
  min-height: 64px;
}

@media (max-width: 900px) {
  .team-hero-inner {
    grid-template-columns: 1fr;
    text-align: center;
    justify-items: center;
  }

  .team-link-row {
    justify-content: center;
  }

  .team-card.team-half {
    grid-column: span 12;
  }
}

@media (max-width: 640px) {
  .team-hero {
    padding: 22px 18px;
  }

  .team-hero h1 {
    font-size: 1.65rem;
  }

  .team-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .team-card,
  .team-card.team-half,
  .team-card.team-full {
    grid-column: span 2;
  }

  .name-chip-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="team-page">

  <section class="team-hero">
    <div class="team-hero-inner">
      <img src="/assets/images/soneya.jpg"
           alt="Dr. Soneya Binta Hossain"
           class="team-pi-photo">

      <div>
        <p class="team-kicker">Principal Investigator</p>
        <h1>Dr. Soneya Binta Hossain</h1>
        <p class="team-titleline">
          Assistant Professor, Computer Science<br>
          University of Texas at Dallas
        </p>
        <p class="team-titleline" style="margin-top:10px;">
          Principal Investigator, <strong>AS²ERT Lab (AI for Safe Software Engineering &amp; Testing)</strong>
        </p>
        <div class="team-link-row">
          <a class="team-button" href="https://assert-lab.github.io/PI/">
            <i class="fas fa-user" aria-hidden="true"></i> Portfolio
          </a>
        </div>
      </div>
    </div>
  </section>

  <div class="team-grid">

    <section class="team-card team-half">
      <h2>PhD Students</h2>
      <div class="member-grid">
        <div class="member-card with-photo">
          <img src="/assets/images/tasfia.jpeg" alt="Tasfia Tasnim">
          <strong class="member-name">Tasfia Tasnim</strong>
          <div class="member-role">
            PhD Student, Computer Science<br>
            University of Texas at Dallas
          </div>
          <div class="member-links">
            <a href="https://scholar.google.com/citations?user=qn2iKXIAAAAJ&amp;hl=en&amp;oi=ao" target="_blank" rel="noopener">Google Scholar</a> ·
            <a href="https://www.linkedin.com/in/tasfia-tasnim-1a52631aa/" target="_blank" rel="noopener">LinkedIn</a>
          </div>
        </div>
      </div>
    </section>

     <section class="team-card team-half">
      <h2>PhD Students</h2>
      <div class="member-grid">
        <div class="member-card with-photo">
          <img src="/assets/images/noshin.jpg" alt="Tasfia Tasnim">
          <strong class="member-name">Noshin Ulfat</strong>
          <div class="member-role">
            PhD Student, Computer Science<br>
            University of Texas at Dallas
          </div>
          <div class="member-links">
            <a href="https://scholar.google.com/citations?user=iDGVVQkAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a> ·
            <a href="https://noshinulfat.github.io/github-portfolio/" target="_blank" rel="noopener">Profile</a>
          </div>
        </div>
      </div>
    </section>

    <section class="team-card team-half">
      <h2>Master’s Students</h2>
      <div class="member-grid">
        <div class="member-card">
          <div class="member-placeholder" aria-hidden="true">N</div>
          <strong class="member-name">Nazia Shehnaz Joynab</strong>
          <div class="member-role">
            MS Student<br>
            University of Texas at Dallas
          </div>
        </div>
      </div>
    </section>

    

    <section class="team-card team-full">
      <h2>Undergraduate Researchers</h2>
      <div class="undergrad-wrapper">

        <section class="semester-card">
          <h3>Spring 2026</h3>
          <div class="name-chip-grid">
            <span class="name-chip">Kartik Kujala</span>
            <span class="name-chip">Atharva Mishra</span>
            <span class="name-chip">Tanishq Seetala</span>
            <span class="name-chip">Kaartik Virigineni</span>
            <span class="name-chip">Pranay Chintakunta</span>
            <span class="name-chip">Davis Mo</span>
            <span class="name-chip">Lokesh Reddy Penugonda</span>
            <span class="name-chip">Madhav Suri</span>
            <span class="name-chip">Akshaj Ande</span>
            <span class="name-chip">Vladislav Kondratyev</span>
            <span class="name-chip">Huzaifa Ahmad Nizami</span>
            <span class="name-chip">Tharun Sevvel</span>
            <span class="name-chip">Sahana Kothuru</span>
            <span class="name-chip">Mahalakshmi Pandian</span>
            <span class="name-chip">Debangshu Pramanik</span>
            <span class="name-chip">Saivishaal Sureshkannan</span>
            <span class="name-chip">Nuzhat Tabassum</span>
            <span class="name-chip">Jaya Vardhini Akurathi</span>
            <span class="name-chip">Joel Preetam Reddy Gurivireddy</span>
            <span class="name-chip">Ali Jafri</span>
            <span class="name-chip">Naksh Jajoo</span>
            <span class="name-chip">Lidege Xi</span>
            <span class="name-chip">Vihan Yerubandi</span>
            <span class="name-chip">Kamsiyochukwu Ozorji</span>
            <span class="name-chip">Krishang Reddy Mandala</span>
            <span class="name-chip">Arnav Kumar</span>
          </div>
        </section>

        <section class="semester-card">
          <h3>Fall 2025</h3>
          <div class="name-chip-grid">
            <span class="name-chip">Aadit Aggarwal</span>
            <span class="name-chip">Jaya Vardhini Akurathi</span>
            <span class="name-chip">Preetham Red Guduri</span>
            <span class="name-chip">Krishang Reddy Mandala</span>
            <span class="name-chip">Debangshu Pramanik</span>
            <span class="name-chip">Ayush Regmi</span>
            <span class="name-chip">Arnav Roy</span>
            <span class="name-chip">Rishi Simhadri</span>
            <span class="name-chip">Ahyaan Syed</span>
            <span class="name-chip">Saivishaal Sureshkannan</span>
            <span class="name-chip">Shyam Venkatesan</span>
            <span class="name-chip">Atharva Mishra</span>
          </div>
        </section>

      </div>
    </section>

    <section class="team-card team-half">
      <h2>High Scool Students</h2>
      <div class="member-grid">
        <div class="member-card">
          <div class="member-placeholder" aria-hidden="true">N</div>
          <strong class="member-name">Shiven Garisa</strong>
          <strong class="member-name">Yash Pamnani</strong>
        </div>
      </div>
    </section>


    <section class="team-card team-full alumni-card">
      <h2>Alumni</h2>
    </section>

  </div>
</div>
