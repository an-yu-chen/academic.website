---
layout: default
title: "Home"
---

<style>
:root {
  --bg: #ffffff;
  --soft-bg: #f6f7fb;
  --text: #1f2937;
  --muted: #6b7280;
  --purple: #6d28d9;
  --green: #065f46;
  --border: #e5e7eb;
}

/* GLOBAL */
body {
  background: var(--bg);
  color: var(--text);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial;
  line-height: 1.7;
}

/* HERO */
.hero {
  text-align: center;
  padding: 90px 20px 60px;
}

.hero h1 {
  font-size: 3rem;
  margin-bottom: 10px;
}

.hero p {
  max-width: 800px;
  margin: 0 auto;
  color: var(--muted);
  font-size: 1.15rem;
}

/* SECTIONS */
.section {
  max-width: 1000px;
  margin: 0 auto;
  padding: 60px 20px;
}

.section h2 {
  font-size: 1.8rem;
  margin-bottom: 25px;
  border-left: 4px solid var(--purple);
  padding-left: 12px;
}

/* EXPERIENCE CARDS */
.card {
  background: white;
  border: 1px solid var(--border);
  padding: 25px;
  border-radius: 12px;
  margin-bottom: 20px;
}

.card h3 {
  margin: 0;
  color: var(--green);
}

.card h4 {
  margin: 5px 0 15px;
  color: var(--muted);
  font-weight: 400;
}

/* =========================
   HORIZONTAL TIMELINE
   ========================= */

.timeline {
  display: flex;
  overflow-x: auto;
  gap: 30px;
  padding: 20px 0;
  scroll-snap-type: x mandatory;
}

.timeline-item {
  min-width: 260px;
  background: var(--soft-bg);
  border: 1px solid var(--border);
  border-radius: 14px;
  padding: 20px;
  scroll-snap-align: start;
  position: relative;
}

.timeline-item h4 {
  color: var(--purple);
  margin: 0 0 10px;
}

.timeline-item p {
  margin: 0;
  color: var(--text);
  font-size: 0.95rem;
}

/* accent dot */
.timeline-item::before {
  content: "";
  width: 10px;
  height: 10px;
  background: var(--green);
  border-radius: 50%;
  position: absolute;
  top: 18px;
  left: 18px;
}
</style>

<div class="hero">
  <h1>An Yu Chen</h1>
  <p>Doctoral Researcher (PhD completed) | Research Associate in Science, Technology & Innovation Policy</p>
</div>

<div class="section">
  <h2>About</h2>
  <p>
    I am a researcher specialising in science of science, innovation policy, and data-driven understanding of technological change. My work focuses on how knowledge flows shape sustainable technologies, AI development, and public policy impact. I am currently based at the University of Manchester, contributing to large-scale research infrastructure and policy-relevant studies.
  </p>
</div>

<div class="section">
  <h2>Research Experience</h2>

  <div class="card">
    <h3>Research Associate</h3>
    <h4>The University of Manchester | 2025–Present</h4>
    <p>
      Working on EPO-funded projects combining bibliometrics, PhD datasets, and computational pipelines using Python, R, and PySpark.
    </p>
  </div>

  <div class="card">
    <h3>Postdoctoral Research (Completed)</h3>
    <h4>Science of Science & Innovation Studies</h4>
    <p>
      Focused on knowledge flows, innovation systems, and empirical policy insights across Europe and the UK.
    </p>
  </div>
</div>

<div class="section">
  <h2>Academic Milestone Timeline</h2>

  <div class="timeline">

    <div class="timeline-item">
      <h4>2026</h4>
      <p>Completed postdoctoral phase in Science of Science research.</p>
    </div>

    <div class="timeline-item">
      <h4>2025–2026</h4>
      <p>Research Associate, University of Manchester (Innovation Policy & Bibliometrics).</p>
    </div>

    <div class="timeline-item">
      <h4>March 2025</h4>
      <p>Visiting Scholar, Politecnico di Milano (Innovation Studies Group).</p>
    </div>

    <div class="timeline-item">
      <h4>2021–2025</h4>
      <p>PhD in Science, Technology and Innovation Policy, Alliance Manchester Business School.</p>
    </div>

    <div class="timeline-item">
      <h4>2024</h4>
      <p>Research Assistant, University of Manchester (data-intensive research projects).</p>
    </div>

    <div class="timeline-item">
      <h4>2023</h4>
      <p>Teaching Assistant – Database Systems.</p>
    </div>

    <div class="timeline-item">
      <h4>2022</h4>
      <p>Early-stage PhD research on knowledge flows and innovation systems.</p>
    </div>

    <div class="timeline-item">
      <h4>2021</h4>
      <p>Started PhD at Alliance Manchester Business School.</p>
    </div>

    <div class="timeline-item">
      <h4>2015</h4>
      <p>MSc in Technology Management, National Tsing Hua University.</p>
    </div>

    <div class="timeline-item">
      <h4>Early Career</h4>
      <p>Developed foundation in data analysis, innovation studies, and research methods.</p>
    </div>

  </div>
</div>

<div class="section">
  <h2>Research Focus</h2>
  <p>
    My research explores the intersection of science, technology, and sustainability, with emphasis on AI, green innovation, and knowledge systems that shape global transitions.
  </p>
</div>
