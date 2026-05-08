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
  padding: 60px 20px 40px;
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
.intro-text {
  max-width: 760px;
  margin: 18px auto 0;
  font-size: 1.02rem;
  color: #4b5563;
  line-height: 1.9;
}

/* SECTION */
.section {
  padding: 35px 20px;
  max-width: 1000px;
  margin: 0 auto;
}

h2 {
  font-size: 1.8rem;
  margin-bottom: 15px;
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
  padding: 20px 10px;
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
  padding: 20px 10px 0px;
}

.connect img {
  width: 330px;
  transition: 0.5s;
}
  
.connect img:hover {
  transform: scale(1.10);
}

/* ===========================
   MAP FIX (removes huge spacing)
   =========================== */

.section.map-section {
  padding-top: 0px;
  padding-bottom: 10px;
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
  margin-bottom: 5px;
}

.action-buttons {
  display: flex;
  justify-content: center;
  gap: 14px;
  margin: 18px 0 10px;
  flex-wrap: wrap;
}

/* base button style */
.btn {
  padding: 10px 18px;
  border-radius: 999px;
  font-size: 0.95rem;
  text-decoration: none;
  font-weight: 500;
  transition: all 0.25s ease;
  border: 1px solid transparent;
}

/* CV button (primary) */
.btn-primary {
  background: #1f2937;
  color: #ffffff;
}

.btn-primary:hover {
  background: #111827;
  transform: translateY(-2px);
}

/* Autobiography button (secondary) */
.btn-secondary {
  background: transparent;
  color: #1f2937;
  border: 1px solid #d1d5db;
}

.btn-secondary:hover {
  background: #f3f4f6;
  transform: translateY(-2px);
}
</style>

<!-- HERO -->
<div class="hero-section">
  <img src="assets/profile_picture.jpg" class="profile-pic">
  <h1>An Yu Chen</h1>
  <p class="subtitle">Innovation Policy & Sustainability Research | Science of Science | PhD in Science, Technology and Innovation Policy (Completed)</p>
  <p class="intro-text">
I am currently working on research projects related to innovation policy, sustainability, environmental economics, and the management of science and technology. My research examines the use and exchange of operant resources among governments, academic institutions, and private firms, drawing upon data from sources including Web of Science, Scopus, and USPTO databases. I aim to continue making a positive impact through excellent research and teaching. Please explore the Research and Teaching sections in the menu for further information. You can always return to this main page by clicking my name, “An Yu Chen,” in the top left corner.
  </p>
</div>
<div class="action-buttons">

  <a href="assets/CV.pdf" target="_blank" class="btn btn-primary">
  View CV
  </a>

  <a href="https://an-yu-chen.github.io/academic.website/autobiography/" class="btn btn-secondary">
  Autobiography
</a>

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
      PhD in Science, Technology and Innovation Policy, University of Manchester (Completed)
      <br>• Supervisors: Professor Cornelia Lawson and Professor Silvia Massini
      <br>• PhD Viva Examiners: Professor Kieron Flanagan and Professor Fabio Montobbio
    </div>

  <div class="timeline-item">
    <div class="timeline-date">2018–2020</div>
    Assistant Editor, Taiwan Hsinchu Industry and Management Forum (Innovation journal publication support and editorial work)
  </div>

  <div class="timeline-item">
    <div class="timeline-date">2017–2020</div>
    Research Assistant, Government Science and Technology Policy Projects (MOST, Taiwan)
    <br>• Analysis of national S&T policy frameworks
    <br>• Evaluation of Taiwan’s science and technology development plans
  </div>

  <div class="timeline-item">
    <div class="timeline-date">2018</div>
    First academic conference presentation: PICMET (Portland International Conference on Management of Engineering and Technology), Honolulu, USA
  </div>

  <div class="timeline-item">
    <div class="timeline-date">2016–2017</div>
    Booking.com — Industry Experience (E-commerce & Tourism Analytics)
  </div>

  <div class="timeline-item">
    <div class="timeline-date">2015</div>
    DAAD Research Internship, Otto-von-Guericke University Magdeburg
    <br>Focus: Human-centered design and emotional product development
  </div>

  <div class="timeline-item">
    <div class="timeline-date">MSc</div>
    MSc in Technology Management, National Tsing Hua University (Institute of Technology Management)
  </div>

  <div class="timeline-item">
    <div class="timeline-date">Early Academic Formation</div>
    Bachelor’s studies in Economics (Arts & Economics background)
    <br>Developed early interest in data, policy, and innovation systems
  </div>

</div>
 

<!-- RESEARCH INTERESTS -->
<div class="section">
  <h2>Research Interests</h2>
  <div class="card">
    Economics of Innovation · Science, Technology & Innovation Policy · Green Technologies · AI for Science · Knowledge Systems & Management · Sustainability Transitions · Digital Transformation of Science
  </div>
</div>

<!-- CONNECT -->
<div class="connect">
  <h2>Connect with Me</h2>
   <p>If you'd like to get in contact with me you can find my LinkedIn or via my email</p>
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
