---
layout: default
title: "Home"
---

<style>
:root {
  --bg: #ffffff;
  --text: #1f2937;
  --muted: #6b7280;
  --purple: #4c1d95;
  --green: #065f46;
  --border: #e5e7eb;
  --card: #f9fafb;
}

body {
  background: var(--bg);
  color: var(--text);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial;
  line-height: 1.7;
  margin: 0;
}

/* HERO */
.hero-section {
  text-align: center;
  padding: 80px 20px 40px;
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
}

.subtitle {
  font-size: 1.2rem;
  color: var(--muted);
}

/* SECTION */
.section {
  padding: 60px 20px;
  max-width: 1000px;
  margin: 0 auto;
}

h2 {
  font-size: 1.8rem;
  margin-bottom: 25px;
  color: var(--purple);
}

/* CARD */
.card {
  background: var(--card);
  border: 1px solid var(--border);
  padding: 25px;
  border-radius: 14px;
}

/* LINKS */
a {
  color: var(--green);
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}

/* ===========================
   TIMELINE (ANIMATED DOTS)
   =========================== */

.timeline {
  position: relative;
  display: flex;
  gap: 20px;
  overflow-x: auto;
  padding: 40px 10px;
  scroll-snap-type: x mandatory;
}

/* center line */
.timeline::before {
  content: "";
  position: absolute;
  top: 70px;
  left: 0;
  right: 0;
  height: 3px;
  background: linear-gradient(90deg, var(--purple), var(--green));
  z-index: 0;
}

.timeline-item {
  position: relative;
  min-width: 260px;
  background: #fff;
  border: 1px solid var(--border);
  border-radius: 12px;
  padding: 20px;
  scroll-snap-align: start;
  z-index: 1;
  transition: transform 0.3s ease;
}

.timeline-item:hover {
  transform: translateY(-5px);
}

/* animated dot */
.timeline-item::before {
  content: "";
  position: absolute;
  top: -18px;
  left: 50%;
  transform: translateX(-50%);
  width: 16px;
  height: 16px;
  border-radius: 50%;
  background: var(--purple);
  border: 3px solid #fff;
  box-shadow: 0 0 0 3px rgba(76, 29, 149, 0.2);
  animation: pulse 2s infinite;
}

.timeline-item:nth-child(even)::before {
  background: var(--green);
  box-shadow: 0 0 0 3px rgba(6, 95, 70, 0.2);
}

@keyframes pulse {
  0% { transform: translateX(-50%) scale(1); }
  50% { transform: translateX(-50%) scale(1.15); }
  100% { transform: translateX(-50%) scale(1); }
}

.timeline-date {
  font-weight: 600;
  margin-bottom: 8px;
  color: var(--purple);
}

/* CONNECT */
.connect {
  text-align: center;
  padding: 90px 50px;
}

.connect img {
  width: 550px;
  transition: 0.5s;
}

/* ===========================
   MAP FIX (removes huge spacing)
   =========================== */

.map-section {
  padding-top: 20px;
  padding-bottom: 40px;
}

/* This is the REAL fix for black/empty space */
#map {
  height: 320px;
  width: 100%;
  border-radius: 14px;
  border: 1px solid #e5e7eb;
  margin: 0;
  padding: 0;
  box-shadow: 0 10px 25px rgba(0,0,0,0.06);
}

/* remove any accidental extra spacing */
.map-section h2 {
  margin-bottom: 10px;
}
</style>

<!-- HERO -->
<div class="hero-section">
  <img src="assets/profile_picture.jpg" class="profile-pic">
  <h1>An Yu Chen</h1>
  <p class="subtitle">Research Associate | Science of Science | PhD (Completed)</p>
</div>

<!-- TIMELINE -->
<div class="section">
  <h2>Academic Milestone Timeline</h2>

  <div class="timeline">

    <div class="timeline-item">
      <div class="timeline-date">2025–2026</div>
      Research Associate in Science of Science, University of Manchester
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
      Research Assistant, MIOIR
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2023</div>
      Teaching Assistant – Database Systems
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2022</div>
      Doctoral research deepened in science of science methods
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2021</div>
      Started PhD at Alliance Manchester Business School
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2015</div>
      MSc in Technology Management completed
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2013–2015</div>
      Graduate studies in Business Administration
    </div>

    <div class="timeline-item">
      <div class="timeline-date">Early Career</div>
      Developed interest in data, policy, and innovation studies
    </div>

  </div>
</div>

<!-- RESEARCH INTERESTS -->
<div class="section">
  <h2>Research Interests</h2>
  <div class="card">
    Science of Science · Innovation Policy · Green Technologies · AI for Science · Knowledge Diffusion · Sustainability Transitions
  </div>
</div>

<!-- CONNECT -->
<div class="connect">
  <h2>Connect with Me</h2>
  <a href="https://www.linkedin.com/in/an-yu-chen">
    <img src="assets/linkedin.png">
  </a>
</div>
<!-- ACADEMIC MAP -->
<div class="section map-section">
  <h2>Academic Network & Global Experience</h2>

  <div id="map"></div>
</div>

<!-- Leaflet Map Library -->
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css">
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<script>
var map = L.map('map').setView([30, 10], 2);

// Base layer (clean academic style)
L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
  attribution: '&copy; OpenStreetMap contributors'
}).addTo(map);

/* ===========================
   ACADEMIC LOCATIONS
   =========================== */

// University of Manchester
L.marker([53.4668, -2.2339]).addTo(map)
  .bindPopup("<b>University of Manchester</b><br>Research Associate");

// Politecnico di Milano
L.marker([45.4781, 9.2266]).addTo(map)
  .bindPopup("<b>Politecnico di Milano</b><br>Visiting Scholar");

// National Tsing Hua University (Taiwan)
L.marker([24.7873, 120.9915]).addTo(map)
  .bindPopup("<b>National Tsing Hua University</b><br>MSc Studies");

// Magdeburg, Germany
L.marker([52.1205, 11.6276]).addTo(map)
  .bindPopup("<b>Magdeburg, Germany</b><br>Research Collaboration / Academic Visits");

// Shanghai, China
L.marker([31.2304, 121.4737]).addTo(map)
  .bindPopup("<b>Shanghai, China</b><br>Research & Academic Connections");

// UI improvement
map.scrollWheelZoom.disable();
</script>
