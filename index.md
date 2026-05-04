---
layout: default
title: "Home"
---

<style>
:root {
  --bg: #ffffff;
  --text: #1f2937;
  --muted: #6b7280;
  --primary: #4c1d95;   /* purple */
  --secondary: #065f46; /* dark green */
  --card: #f9fafb;
  --border: #e5e7eb;
}

body {
  background: var(--bg);
  color: var(--text);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial;
  line-height: 1.7;
}

/* HERO */
.hero-section {
  text-align: center;
  padding: 80px 20px;
  background: #ffffff;
}

.profile-pic {
  width: 240px;
  height: 240px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #fff;
  box-shadow: 0 10px 30px rgba(0,0,0,0.08);
}

h1 {
  font-size: 3rem;
  margin: 20px 0 5px;
  color: var(--text);
}

.subtitle {
  font-size: 1.2rem;
  color: var(--muted);
}

/* SECTIONS */
.section {
  padding: 60px 20px;
  max-width: 1000px;
  margin: 0 auto;
}

h2 {
  font-size: 1.8rem;
  margin-bottom: 25px;
  color: var(--primary);
}

/* CARDS */
.card {
  background: var(--card);
  border: 1px solid var(--border);
  padding: 25px;
  border-radius: 14px;
  margin-bottom: 20px;
}

/* TEXT */
p {
  color: var(--text);
}

/* LINKS */
a {
  color: var(--secondary);
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}

/* ===========================
   HORIZONTAL TIMELINE
   =========================== */

.timeline {
  display: flex;
  overflow-x: auto;
  gap: 20px;
  padding: 20px 10px;
  scroll-snap-type: x mandatory;
}

.timeline-item {
  min-width: 260px;
  background: #ffffff;
  border: 2px solid var(--border);
  border-top: 4px solid var(--primary);
  border-radius: 12px;
  padding: 20px;
  scroll-snap-align: start;
  position: relative;
}

.timeline-item:nth-child(even) {
  border-top-color: var(--secondary);
}

.timeline-date {
  font-weight: 600;
  color: var(--primary);
  margin-bottom: 8px;
}

/* LINKEDIN */
.connect {
  text-align: center;
  padding: 50px 20px;
}

.connect img {
  width: 220px;
  transition: 0.3s;
}

.connect img:hover {
  transform: scale(1.05);
}
</style>

<!-- HERO -->
<div class="hero-section">
  <img src="assets/profile_picture.jpg" class="profile-pic">
  <h1>An Yu Chen</h1>
  <p class="subtitle">Research Associate | Science of Science | PhD (Completed)</p>
</div>

<!-- ABOUT -->
<div class="section">
  <h2>About</h2>
  <div class="card">
    <p>
      I am a researcher at the University of Manchester working on science of science, innovation policy, and knowledge flows.
      My work explores how scientific knowledge translates into sustainable technologies and informs public policy, particularly in green innovation and AI.
    </p>
  </div>
</div>

<!-- RESEARCH -->
<div class="section">
  <h2>Research Experience</h2>

  <div class="card">
    <strong>Research Associate</strong><br>
    University of Manchester (2025–Present)<br><br>
    Working on EPO-funded projects linking bibliometric and doctoral datasets to understand knowledge production and diffusion.
  </div>
</div>

<!-- TIMELINE -->
<div class="section">
  <h2>Academic Milestone Timeline</h2>

  <div class="timeline">

    <div class="timeline-item">
      <div class="timeline-date">2025–2026</div>
      Research Associate in Science of Science at the University of Manchester
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2021–2025</div>
      PhD in Science, Technology and Innovation Policy (Completed)
    </div>

    <div class="timeline-item">
      <div class="timeline-date">March 2025</div>
      Visiting Scholar, Politecnico di Milano
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2023–2024</div>
      Research Assistant, MIOIR, AMBS
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2023</div>
      Teaching Assistant – Database Systems
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2019–2020</div>
      Research Internship in Innovation Studies
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2018</div>
      Early research exposure in data science methods
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2015</div>
      MSc in Technology Management (Completed)
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2013–2015</div>
      Graduate studies in Business Administration
    </div>

    <div class="timeline-item">
      <div class="timeline-date">Early Career</div>
      Developed foundational interest in science, policy, and data
    </div>

  </div>
</div>

<!-- RESEARCH INTERESTS -->
<div class="section">
  <h2>Research Interests</h2>
  <div class="card">
    Science of science · Innovation policy · Green technologies · AI for science · Knowledge diffusion · Sustainability transitions
  </div>
</div>

<!-- CONNECT -->
<div class="connect">
  <h2>Connect</h2>
  <a href="https://www.linkedin.com/">
    <img src="assets/linkedin.png">
  </a>
</div>
