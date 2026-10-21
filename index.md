
---
layout: default
title: "Home"
---

<!-- GOOGLE FONTS -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<!-- LEAFLET MAP -->
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css">

<style>
/* =========================================
   COLOUR PALETTE & GLOBAL STYLES
   ========================================= */

:root {
  --blue: #164e9a;
  --blue-dark: #103568;
  --blue-deep: #0b2345;
  --blue-light: #eaf2ff;
  --blue-pale: #f4f8ff;

  --yellow: #ffd447;
  --yellow-light: #fff5c9;

  --white: #ffffff;
  --text: #243247;
  --muted: #66758a;
  --border: #dce5f1;
  --card: #ffffff;

  --shadow-sm: 0 5px 18px rgba(16, 53, 104, 0.06);
  --shadow-md: 0 12px 32px rgba(16, 53, 104, 0.10);
  --shadow-lg: 0 20px 45px rgba(16, 53, 104, 0.14);

  --radius: 18px;
}

html {
  scroll-behavior: smooth;
}

body {
  background: var(--white);
  color: var(--text);
  font-family: "DM Sans", sans-serif;
  font-size: 16px;
  line-height: 1.8;
  margin: 0;
  -webkit-font-smoothing: antialiased;
}

* {
  box-sizing: border-box;
}

img {
  max-width: 100%;
}

a {
  color: var(--blue);
  text-decoration: none;
  transition: color 0.25s ease;
}

a:hover {
  color: var(--blue-dark);
}

::selection {
  background: var(--yellow);
  color: var(--blue-deep);
}

/* =========================================
   HERO SECTION
   ========================================= */

.hero-section {
  position: relative;
  overflow: hidden;
  text-align: center;
  padding: 78px 24px 58px;
  background:
    radial-gradient(
      circle at 10% 15%,
      rgba(255, 212, 71, 0.20),
      transparent 25%
    ),
    radial-gradient(
      circle at 90% 75%,
      rgba(89, 151, 237, 0.13),
      transparent 28%
    ),
    linear-gradient(180deg, #f4f8ff 0%, #ffffff 100%);
}

/* Decorative yellow accent */
.hero-section::before {
  content: "";
  position: absolute;
  top: 38px;
  right: max(calc((100% - 950px) / 2), 35px);
  width: 62px;
  height: 7px;
  background: var(--yellow);
  border-radius: 20px;
  transform: rotate(-35deg);
}

.hero-section::after {
  content: "";
  position: absolute;
  bottom: 50px;
  left: max(calc((100% - 950px) / 2), 35px);
  width: 16px;
  height: 16px;
  background: var(--yellow);
  border-radius: 50%;
  opacity: 0.85;
}

.profile-pic {
  display: block;
  width: 230px;
  height: 230px;
  margin: 0 auto;
  border-radius: 24px;
  object-fit: cover;
  object-position: center;
  border: 5px solid var(--white);
  outline: 1px solid var(--border);
  box-shadow: var(--shadow-lg);
  transition:
    transform 0.4s ease,
    box-shadow 0.4s ease;
}

.profile-pic:hover {
  transform: translateY(-5px) rotate(-1deg);
  box-shadow: 0 24px 50px rgba(22, 78, 154, 0.20);
}

.hero-section h1 {
  margin: 27px 0 10px;
  color: var(--blue-deep);
  font-family: "Manrope", sans-serif;
  font-size: clamp(2.4rem, 5vw, 3.8rem);
  font-weight: 800;
  letter-spacing: -2px;
  line-height: 1.2;
}

.subtitle {
  max-width: 850px;
  margin: 0 auto;
  color: var(--blue);
  font-family: "Manrope", sans-serif;
  font-size: clamp(1rem, 2vw, 1.18rem);
  font-weight: 600;
  line-height: 1.8;
}

.intro-text {
  max-width: 780px;
  margin: 24px auto 0;
  color: var(--muted);
  font-size: 1.02rem;
  line-height: 2;
}

/* =========================================
   ACTION BUTTONS
   ========================================= */

.action-buttons {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 16px;
  flex-wrap: wrap;
  margin: -3px 20px 42px;
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  padding: 12px 24px;
  border-radius: 999px;
  font-family: "Manrope", sans-serif;
  font-size: 0.95rem;
  font-weight: 700;
  text-decoration: none;
  transition:
    transform 0.25s ease,
    box-shadow 0.25s ease,
    background 0.25s ease;
}

.btn-primary {
  background: var(--blue);
  color: var(--white);
  border: 2px solid var(--blue);
  box-shadow: 0 6px 16px rgba(22, 78, 154, 0.16);
}

.btn-primary:hover {
  background: var(--blue-dark);
  color: var(--white);
  transform: translateY(-3px);
  box-shadow: 0 10px 24px rgba(22, 78, 154, 0.22);
}

.btn-secondary {
  background: var(--white);
  color: var(--blue-dark);
  border: 2px solid var(--border);
}

.btn-secondary:hover {
  background: var(--yellow-light);
  color: var(--blue-dark);
  border-color: var(--yellow);
  transform: translateY(-3px);
}

/* =========================================
   GENERAL SECTIONS
   ========================================= */

.section {
  width: min(100% - 48px, 1050px);
  margin: 0 auto;
  padding: 46px 0;
}

.section h2,
.connect h2 {
  position: relative;
  margin: 0 0 26px;
  padding-bottom: 14px;
  color: var(--blue-dark);
  font-family: "Manrope", sans-serif;
  font-size: clamp(1.55rem, 3vw, 2rem);
  font-weight: 800;
  letter-spacing: -0.7px;
  line-height: 1.4;
}

/* Short yellow heading underline */
.section h2::after,
.connect h2::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  width: 58px;
  height: 5px;
  border-radius: 10px;
  background: var(--yellow);
}

.card {
  padding: 30px 32px;
  background: var(--card);
  border: 1px solid var(--border);
  border-radius: var(--radius);
  box-shadow: var(--shadow-sm);
  transition:
    box-shadow 0.3s ease,
    border-color 0.3s ease;
}

.card:hover {
  border-color: #c4d7f4;
  box-shadow: var(--shadow-md);
}

/* =========================================
   ACADEMIC TIMELINE
   ========================================= */

.timeline {
  position: relative;
  display: flex;
  gap: 22px;
  overflow-x: auto;
  padding: 28px 12px 30px;
  scroll-snap-type: x mandatory;
  scrollbar-width: thin;
  scrollbar-color: #b8cbea #f0f4fa;
  overscroll-behavior-x: contain;
}

/* Timeline centre line */
.timeline::before {
  content: "";
  position: absolute;
  top: 76px;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(
    90deg,
    var(--blue),
    #76a8e8,
    var(--yellow)
  );
  border-radius: 20px;
  z-index: 0;
}

.timeline-item {
  position: relative;
  flex: 0 0 280px;
  min-width: 0;
  align-self: stretch;
  padding: 27px 23px 25px;
  background: var(--white);
  border: 1px solid var(--border);
  border-top: 4px solid var(--blue);
  border-radius: 15px;
  box-shadow: var(--shadow-sm);
  font-size: 0.96rem;
  line-height: 1.85;
  scroll-snap-align: start;
  z-index: 1;
  transition:
    transform 0.3s ease,
    box-shadow 0.3s ease,
    border-color 0.3s ease;
}

.timeline-item:nth-child(even) {
  border-top-color: var(--yellow);
}

.timeline-item:hover {
  transform: translateY(-6px);
  box-shadow: var(--shadow-md);
  border-color: #c4d7f4;
}

/* Timeline dots */
.timeline-item::before {
  content: "";
  position: absolute;
  top: -19px;
  left: 50%;
  transform: translateX(-50%);
  width: 15px;
  height: 15px;
  border-radius: 50%;
  background: var(--blue);
  border: 3px solid var(--white);
  box-shadow: 0 0 0 3px rgba(22, 78, 154, 0.16);
  animation: timeline-pulse 2.5s ease-in-out infinite;
}

.timeline-item:nth-child(even)::before {
  background: #e5ad00;
  box-shadow: 0 0 0 3px rgba(255, 212, 71, 0.35);
}

.timeline-date {
  margin-bottom: 12px;
  color: var(--blue);
  font-family: "Manrope", sans-serif;
  font-size: 1rem;
  font-weight: 800;
  line-height: 1.5;
}

.timeline-item:nth-child(even) .timeline-date {
  color: #866300;
}

.timeline-item a {
  display: inline-block;
  margin-top: 4px;
  font-weight: 700;
}

@keyframes timeline-pulse {
  0%, 100% {
    box-shadow: 0 0 0 3px rgba(22, 78, 154, 0.15);
  }

  50% {
    box-shadow: 0 0 0 7px rgba(22, 78, 154, 0.05);
  }
}

.timeline-item:nth-child(even) {
  --timeline-dot: var(--yellow);
}

/* =========================================
   RESEARCH INTERESTS
   ========================================= */

.card ul {
  margin: 0;
  padding-left: 24px;
}

.card li {
  padding: 7px 0 7px 5px;
  color: var(--text);
  line-height: 1.9;
}

.card li::marker {
  color: var(--blue);
}

.card li::selection {
  background: var(--yellow);
}

/* =========================================
   CONNECT SECTION
   ========================================= */

.connect {
  position: relative;
  margin-top: 30px;
  padding: 48px 24px 45px;
  text-align: center;
  background:
    radial-gradient(
      circle at 15% 50%,
      rgba(255, 212, 71, 0.18),
      transparent 22%
    ),
    linear-gradient(135deg, #f4f8ff, #ffffff);
  border-top: 1px solid var(--border);
  border-bottom: 1px solid var(--border);
}

.connect h2 {
  display: inline-block;
  margin-bottom: 12px;
}

.connect h2::after {
  left: 50%;
  transform: translateX(-50%);
}

.connect p {
  margin: 8px auto 22px;
  color: var(--muted);
  font-size: 1rem;
}

.connect a {
  display: inline-block;
  line-height: 0;
}

.connect img {
  display: block;
  width: 230px;
  max-width: 80vw;
  height: auto;
  margin: 0 auto;
  border-radius: 12px;
  transition:
    transform 0.3s ease,
    filter 0.3s ease;
}

.connect img:hover {
  transform: translateY(-4px) scale(1.03);
  filter: drop-shadow(0 8px 12px rgba(22, 78, 154, 0.12));
}

/* =========================================
   ACADEMIC NETWORK MAP
   ========================================= */

.section.map-section {
  padding-top: 45px;
  padding-bottom: 55px;
}

.map-section h2 {
  margin-bottom: 18px;
}

#map {
  display: block;
  width: 100%;
  height: 350px;
  margin: 0;
  padding: 0;
  border: 1px solid var(--border);
  border-radius: var(--radius);
  background: var(--blue-pale);
  box-shadow: var(--shadow-md);
  z-index: 1;
}

/* Map popups */
.leaflet-popup-content-wrapper {
  border-radius: 12px;
  font-family: "DM Sans", sans-serif;
}

.leaflet-popup-content {
  line-height: 1.7;
}

.leaflet-popup-content b {
  color: var(--blue-dark);
  font-family: "Manrope", sans-serif;
}

/* =========================================
   ACCESSIBILITY & RESPONSIVE DESIGN
   ========================================= */

a:focus-visible,
button:focus-visible {
  outline: 3px solid #d8a900;
  outline-offset: 4px;
}

@media (max-width: 768px) {
  .hero-section {
    padding: 54px 22px 42px;
  }

  .hero-section::before {
    right: 25px;
    top: 22px;
    width: 42px;
  }

  .hero-section::after {
    left: 25px;
    bottom: 25px;
  }

  .profile-pic {
    width: 190px;
    height: 190px;
    border-radius: 20px;
  }

  .hero-section h1 {
    letter-spacing: -1.2px;
  }

  .intro-text {
    font-size: 0.98rem;
    line-height: 1.85;
  }

  .action-buttons {
    margin-bottom: 25px;
    gap: 12px;
  }

  .btn {
    padding: 11px 19px;
  }

  .section {
    width: calc(100% - 36px);
    padding: 32px 0;
  }

  .section h2,
  .connect h2 {
    font-size: 1.55rem;
  }

  .card {
    padding: 23px 20px;
  }

  .timeline {
    gap: 16px;
    padding-left: 8px;
    padding-right: 8px;
  }

  .timeline-item {
    flex-basis: 265px;
    padding: 24px 20px;
  }

  .timeline::before {
    top: 76px;
  }

  .connect {
    padding: 38px 20px;
  }

  .section.map-section {
    padding-top: 32px;
    padding-bottom: 38px;
  }

  #map {
    height: 300px;
  }
}

@media (max-width: 420px) {
  .profile-pic {
    width: 165px;
    height: 165px;
  }

  .hero-section h1 {
    font-size: 2.25rem;
  }

  .subtitle {
    font-size: 0.95rem;
  }

  .action-buttons {
    flex-direction: column;
    align-items: stretch;
    margin-left: 24px;
    margin-right: 24px;
  }

  .btn {
    width: 100%;
  }

  .timeline-item {
    flex-basis: 245px;
  }

  #map {
    height: 270px;
  }
}

/* Respect reduced-motion preferences */
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    scroll-behavior: auto !important;
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
</style>

<!-- =========================================
     HERO / PROFILE
     ========================================= -->

<div class="hero-section">

  <img
    src="assets/profile_picture.jpg"
    class="profile-pic"
    alt="Profile photo of An Yu Chen"
  >

  <h1>An Yu Chen</h1>

  <p class="subtitle">
    Innovation Policy &amp; Sustainability Research |
    Science of Science |
    PhD in Science, Technology and Innovation Policy (Completed)
  </p>

  <p class="intro-text">
    I am currently working on research projects related to innovation policy,
    sustainability, environmental economics, and the management of science
    and technology. My research examines the use and exchange of operant
    resources among governments, academic institutions, and private firms,
    drawing upon data from sources including Web of Science, Scopus, and
    USPTO databases. I aim to continue making a positive impact through
    excellent research and teaching. Please explore the Research and
    Teaching sections in the menu for further information. You can always
    return to this main page by clicking my name, “An Yu Chen,” in the top
    left corner.
  </p>

</div>

<!-- =========================================
     CV & AUTOBIOGRAPHY
     ========================================= -->

<div class="action-buttons">

  <a
    href="assets/CV.pdf"
    target="_blank"
    rel="noopener noreferrer"
    class="btn btn-primary"
  >
    View CV ↗
  </a>

  <a
    href="https://an-yu-chen.github.io/academic.website/autobiography/"
    class="btn btn-secondary"
  >
    Autobiography →
  </a>

</div>

<!-- =========================================
     ACADEMIC MILESTONE TIMELINE
     ========================================= -->

<div class="section">

  <h2>Academic Milestone Timeline</h2>

  <div class="timeline">

    <div class="timeline-item">

      <div class="timeline-date">September 2026</div>

      Contributed to WIPO’s <em>Women, Innovation and Impact</em> booklet

      <br><br>

      <a
        href="https://www.wipo.int/publications/en/details.jsp?id=4879"
        target="_blank"
        rel="noopener noreferrer"
      >
        View the WIPO publication →
      </a>

    </div>

    <div class="timeline-item">

      <div class="timeline-date">2025–2026</div>

      Research Associate in Science of Science, University of Manchester

    </div>

    <div class="timeline-item">

      <div class="timeline-date">2021–2026</div>

      PhD in Science, Technology and Innovation Policy, University of
      Manchester (Completed)

      <br>
      • Supervisors: Professor Cornelia Lawson and Professor Silvia Massini

      <br>
      • PhD Viva Examiners: Professor Kieron Flanagan and Professor Fabio
      Montobbio

    </div>

    <div class="timeline-item">

      <div class="timeline-date">2018–2020</div>

      Assistant Editor, Taiwan Hsinchu Industry and Management Forum
      (Innovation journal publication support and editorial work)

    </div>

    <div class="timeline-item">

      <div class="timeline-date">2017–2020</div>

      Research Assistant, Government Science and Technology Policy Projects
      (MOST, Taiwan)

      <br>
      • Analysis of national S&amp;T policy frameworks

      <br>
      • Evaluation of Taiwan’s science and technology development plans

    </div>

    <div class="timeline-item">

      <div class="timeline-date">2018</div>

      First academic conference presentation: PICMET (Portland International
      Conference on Management of Engineering and Technology), Honolulu, USA

    </div>

    <div class="timeline-item">

      <div class="timeline-date">2016–2017</div>

      Booking.com — Industry Experience (E-commerce &amp; Tourism Analytics)

    </div>

    <div class="timeline-item">

      <div class="timeline-date">2015</div>

      DAAD Research Internship, Otto-von-Guericke University Magdeburg

      <br>

      Focus: Human-centered design and emotional product development

    </div>

    <div class="timeline-item">

      <div class="timeline-date">MSc</div>

      MSc in Technology Management, National Tsing Hua University
      (Institute of Technology Management)

    </div>

    <div class="timeline-item">

      <div class="timeline-date">Early Academic Formation</div>

      Bachelor’s studies in Economics (Arts &amp; Economics background)

      <br>

      Developed early interest in data, policy, and innovation systems

    </div>

  </div>

</div>

<!-- =========================================
     RESEARCH INTERESTS
     ========================================= -->

<div class="section">

  <h2>Research Interests and Areas of Practice</h2>

  <div class="card">

    <ul>

      <li>
        Economics of Innovation with a focus on technological change,
        knowledge creation, and the dynamics of emerging industries
      </li>

      <li>
        Science, Technology &amp; Innovation Policy examining research
        ecosystems
      </li>

      <li>
        Green Technologies and Sustainable Innovation addressing
        environmental transitions
      </li>

      <li>
        Critical reflection on AI, systems, and contemporary digital life
      </li>

      <li>
        Digital Transformation of Science analysing the impact of digital
        infrastructures, computational methods, and intelligent technologies
        on scientific practice, collaboration, and innovation processes
      </li>

    </ul>

  </div>

</div>

<!-- =========================================
     CONNECT WITH ME
     ========================================= -->

<div class="connect">

  <h2>Connect with Me</h2>

  <p>
    If you'd like to get in contact with me you can find my LinkedIn or
    via my email
  </p>

  <a
    href="https://www.linkedin.com/in/an-yu-chen"
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Visit An Yu Chen's LinkedIn profile"
  >

    <img
      src="assets/linkedin.png"
      alt="LinkedIn"
      loading="lazy"
    >

  </a>

</div>

<!-- =========================================
     ACADEMIC NETWORK & GLOBAL EXPERIENCE
     ========================================= -->

<div class="section map-section">

  <h2>Academic Network &amp; Global Experience</h2>

  <div
    id="map"
    role="application"
    aria-label="Interactive map showing academic locations in the United Kingdom, Italy, Taiwan, Germany and China"
  ></div>

</div>

<!-- =========================================
     LEAFLET MAP SCRIPT
     ========================================= -->

<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<script>
(function () {
  function initializeAcademicMap() {
    var mapElement = document.getElementById("map");

    if (!mapElement || typeof L === "undefined") {
      return;
    }

    // Avoid creating the map more than once.
    if (mapElement._leaflet_id) {
      return;
    }

    // Initial global view.
    var map = L.map("map", {
      scrollWheelZoom: false,
      zoomControl: true
    }).setView([30, 10], 2);

    // OpenStreetMap base layer.
    L.tileLayer(
      "https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",
      {
        attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap contributors</a>',
        maxZoom: 19
      }
    ).addTo(map);

    // University of Manchester.
    L.marker([53.4668, -2.2339])
      .addTo(map)
      .bindPopup(
        "<b>University of Manchester</b><br>Research Associate"
      );

    // Politecnico di Milano.
    L.marker([45.4781, 9.2266])
      .addTo(map)
      .bindPopup(
        "<b>Politecnico di Milano</b><br>Visiting Scholar"
      );

    // National Tsing Hua University, Taiwan.
    L.marker([24.7873, 120.9915])
      .addTo(map)
      .bindPopup(
        "<b>National Tsing Hua University</b><br>MSc Studies"
      );

    // Magdeburg, Germany.
    L.marker([52.1205, 11.6276])
      .addTo(map)
      .bindPopup(
        "<b>Magdeburg, Germany</b><br>Research Collaboration / Academic Visits"
      );

    // Shanghai, China.
    L.marker([31.2304, 121.4737])
      .addTo(map)
      .bindPopup(
        "<b>Shanghai, China</b><br>Research &amp; Academic Connections"
      );

    // Prevent a blank map when its container finishes rendering.
    setTimeout(function () {
      map.invalidateSize();
    }, 100);
  }

  if (document.readyState === "loading") {
    document.addEventListener(
      "DOMContentLoaded",
      initializeAcademicMap
    );
  } else {
    initializeAcademicMap();
  }
})();
</script>
