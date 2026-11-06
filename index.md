---
layout: default
title: "Home"
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css">

<style>
:root {
  --ab: #073d7b;
  --am: #0756a5;
  --ay: #ffd633;
  --ap: #fff9e8;
  --ink: #17385d;
  --muted: #56708c;
  --line: #e1eaf3;
}

.academic-home {
  color: var(--ink);
  font-family: "DM Sans", "Segoe UI", sans-serif;
  font-size: 16px;
  line-height: 1.75;
  -webkit-font-smoothing: antialiased;
}
.academic-home *,
.academic-home *::before,
.academic-home *::after { box-sizing: border-box; }
.academic-home a { color: var(--am); text-decoration: none; }
.academic-home a:hover { color: var(--ab); text-decoration: underline; text-underline-offset: 3px; }

.academic-hero {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow: hidden;
  padding: clamp(42px, 6vw, 72px) 24px 38px;
  background: #fff;
  text-align: center;
}
.academic-hero::before {
  position: absolute;
  top: 27px;
  left: calc(50% - 32px);
  width: 64px;
  height: 5px;
  border-radius: 8px;
  background: var(--ay);
  content: "";
}
.academic-hero::after {
  position: absolute;
  top: 45px;
  right: max(calc((100% - 1000px) / 2), 22px);
  width: 14px;
  height: 14px;
  border-radius: 50%;
  background: var(--ay);
  content: "";
  pointer-events: none;
}
.academic-profile-wrap {
  position: relative;
  z-index: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.academic-profile {
  display: block;
  width: clamp(175px, 21vw, 225px);
  height: clamp(175px, 21vw, 225px);
  aspect-ratio: 1;
  border: 5px solid #fff;
  border-radius: 50%;
  outline: 2px solid var(--line);
  object-fit: cover;
  object-position: center;
  box-shadow: 0 12px 34px #073d7b18;
}
.academic-profile-caption {
  display: inline-block;
  margin-top: 16px;
  padding: 7px 14px;
  border: 1px solid #ffeb9a;
  border-radius: 999px;
  background: #fff8d9;
  color: var(--ab);
  font-size: .8rem;
  font-weight: 700;
}
.academic-eyebrow {
  margin: 27px 0 0;
  color: var(--am);
  font-size: .78rem;
  font-weight: 800;
  letter-spacing: .14em;
  text-transform: uppercase;
}
.academic-hero h1 {
  margin: 10px 0 9px;
  color: var(--ab);
  font: 800 clamp(2.4rem, 5vw, 4.1rem)/1.08 "Manrope", sans-serif;
  letter-spacing: -.045em;
}
.academic-subtitle {
  max-width: 850px;
  margin: 0;
  color: var(--am);
  font: 700 clamp(1rem, 2vw, 1.18rem)/1.7 "Manrope", sans-serif;
}
.academic-rule {
  width: 58px;
  height: 5px;
  margin: 19px auto 16px;
  border-radius: 8px;
  background: var(--ay);
}
.academic-intro {
  max-width: 820px;
  margin: 0 auto;
  color: var(--muted);
  line-height: 1.9;
}

.academic-actions {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 12px;
  padding: 22px 18px 8px;
}
.academic-btn {
  display: inline-flex;
  min-height: 46px;
  align-items: center;
  justify-content: center;
  padding: 10px 21px;
  border: 2px solid var(--ab);
  border-radius: 999px;
  font: 800 .92rem "Manrope", sans-serif;
  transition: transform .2s, box-shadow .2s;
}
.academic-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 30px #073d7b14;
  text-decoration: none !important;
}
.academic-btn-primary { background: var(--ab); color: #fff !important; }
.academic-btn-secondary { border-color: var(--line); background: #fff; color: var(--ab) !important; }
.academic-btn-secondary:hover { border-color: var(--ay); background: var(--ap); }

.academic-section {
  width: min(100% - 44px, 1160px);
  margin: 0 auto;
  padding: 39px 0;
}
.academic-section-title {
  display: flex;
  align-items: center;
  gap: 14px;
  margin: 0 0 22px;
  color: var(--ab);
  font: 800 clamp(1.45rem, 3vw, 1.9rem)/1.3 "Manrope", sans-serif;
  letter-spacing: -.025em;
}
.academic-section-title::before {
  flex: 0 0 45px;
  height: 5px;
  border-radius: 8px;
  background: var(--ay);
  content: "";
}

.academic-highlight {
  display: grid;
  grid-template-columns: 82px 1fr;
  align-items: center;
  gap: 22px;
  padding: clamp(22px, 3vw, 30px);
  border: 1px solid #ffefb2;
  border-radius: 16px;
  background: var(--ap);
}
.academic-highlight-icon {
  display: grid;
  width: 70px;
  height: 70px;
  place-items: center;
  border: 2px solid var(--ab);
  border-radius: 50%;
  background: #fff;
  color: var(--ab);
  font-size: 32px;
  box-shadow: 6px 6px 0 var(--ay);
}
.academic-highlight-copy { padding-left: 22px; border-left: 3px solid var(--ay); }
.academic-highlight h2 {
  margin: 0 0 8px;
  color: var(--ab);
  font: 800 1.3rem "Manrope", sans-serif;
}
.academic-highlight p { margin: 0; }

.academic-interest-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 17px;
}
.academic-interest {
  padding: 23px 22px;
  border: 1px solid var(--line);
  border-radius: 15px;
  background: #fff;
  box-shadow: 0 5px 16px #1035680a;
  transition: transform .25s, border-color .25s, box-shadow .25s;
}
.academic-interest:hover {
  transform: translateY(-4px);
  border-color: #bfd4f0;
  box-shadow: 0 10px 30px #073d7b14;
}
.academic-interest-icon {
  display: grid;
  width: 46px;
  height: 46px;
  margin-bottom: 14px;
  place-items: center;
  border-radius: 14px;
  background: var(--ay);
  color: var(--ab);
  font-size: 22px;
  font-weight: 800;
}
.academic-interest h3 {
  margin: 0 0 8px;
  color: var(--ab);
  font: 800 1.04rem/1.4 "Manrope", sans-serif;
}
.academic-interest p { margin: 0; color: var(--muted); font-size: .92rem; line-height: 1.7; }

.academic-timeline {
  display: flex;
  gap: 20px;
  overflow-x: auto;
  padding: 12px 8px 24px;
  scroll-snap-type: x mandatory;
  scrollbar-color: #b8cbea #f0f4fa;
  scrollbar-width: thin;
}
.academic-timeline-item {
  flex: 0 0 280px;
  padding: 24px 22px;
  border: 1px solid var(--line);
  border-top: 4px solid var(--ab);
  border-radius: 15px;
  background: #fff;
  box-shadow: 0 5px 18px #1035680d;
  font-size: .92rem;
  line-height: 1.75;
  scroll-snap-align: start;
}
.academic-timeline-item:nth-child(even) { border-top-color: var(--ay); }
.academic-timeline-date {
  display: block;
  margin-bottom: 9px;
  color: var(--ab);
  font: 800 1rem "Manrope", sans-serif;
}
.academic-timeline-item {
  position: relative;
  overflow: hidden;
}

.academic-timeline-item::after {
  content: "";
  position: absolute;
  top: 18px;
  right: 18px;
  width: 9px;
  height: 9px;
  border-radius: 50%;
  background: #ffd633;
  box-shadow:
    0 0 5px #ffd633,
    0 0 12px #ffd633,
    0 0 22px #ffd633;
  animation: academic-shine 2s ease-in-out infinite;
}

@keyframes academic-shine {
  0%, 100% {
    opacity: 0.45;
    transform: scale(0.8);
    box-shadow: 0 0 4px #ffd633;
  }

  50% {
    opacity: 1;
    transform: scale(1.25);
    box-shadow:
      0 0 7px #ffd633,
      0 0 15px #ffd633,
      0 0 25px #ffd633;
  }
}

@media (prefers-reduced-motion: reduce) {
  .academic-timeline-item::after {
    animation: none;
    opacity: 1;
  }
}
.academic-graduation-photo {
  display: block;
  width: 110px;
  height: auto;
  max-height: 130px;
  margin-top: 14px;
  border: 2px solid var(--line);
  border-radius: 9px;
  object-fit: cover;
  object-position: center;
  box-shadow: 0 4px 12px #073d7b14;
}
.academic-timeline-item:nth-child(even) .academic-timeline-date { color: #806000; }
.academic-timeline-item a { display: inline-block; margin-top: 8px; font-weight: 700; }

.academic-card {
  padding: clamp(22px, 3vw, 34px);
  border: 1px solid var(--line);
  border-radius: 17px;
  background: #fff;
  box-shadow: 0 5px 18px #1035680b;
}
.academic-card p:first-child { margin-top: 0; }
.academic-card p:last-child { margin-bottom: 0; }

.academic-contact {
  margin-top: 10px;
  padding: 42px 24px;
  border-block: 1px solid var(--line);
  background: linear-gradient(115deg, #f3f8ff, #fffdf5);
  text-align: center;
}
.academic-contact h2 {
  margin: 0 0 10px;
  color: var(--ab);
  font: 800 1.8rem "Manrope", sans-serif;
}
.academic-contact h2::after {
  display: block;
  width: 55px;
  height: 4px;
  margin: 12px auto;
  border-radius: 8px;
  background: var(--ay);
  content: "";
}
.academic-contact p { color: var(--muted); }
.academic-social {
  display: inline-block;
  margin-top: 6px;
  padding: 10px 18px;
  border-radius: 999px;
  background: var(--ab);
  color: #fff !important;
  font-weight: 800;
}
.academic-social:hover { background: var(--am); text-decoration: none !important; }

.academic-map {
  z-index: 1;
  width: 100%;
  height: 350px;
  border: 1px solid var(--line);
  border-radius: 16px;
  background: #eaf2ff;
  box-shadow: 0 10px 30px #073d7b14;
}
.academic-map-note { margin: 10px 0 0; color: var(--muted); font-size: .82rem; }

@media (max-width: 800px) {
  .academic-hero { padding-top: 58px; }
  .academic-hero::after { top: 30px; right: 24px; }
  .academic-profile { width: 175px; height: 175px; }
  .academic-interest-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
}
@media (max-width: 540px) {
  .academic-section { width: calc(100% - 32px); padding: 30px 0; }
  .academic-hero { padding: 54px 22px 32px; }
  .academic-profile { width: 150px; height: 150px; }
  .academic-highlight { grid-template-columns: 1fr; gap: 16px; }
  .academic-highlight-copy { padding-left: 16px; }
  .academic-interest-grid { grid-template-columns: 1fr; }
  .academic-timeline-item { flex-basis: 250px; }
  .academic-map { height: 290px; }
}
@media (prefers-reduced-motion: reduce) {
  .academic-home *,
  .academic-home *::before,
  .academic-home *::after {
    scroll-behavior: auto !important;
    transition-duration: .01ms !important;
  }
}
</style>

<div class="academic-home">

  <!-- INTRODUCTION -->
  <section class="academic-hero">
    <div class="academic-profile-wrap">
      <img
        src="{{ '/assets/profile_picture.jpg' | relative_url }}"
        class="academic-profile"
        alt="Portrait of Dr An Yu Chen"
        loading="eager"
      >
      <span class="academic-profile-caption">Welcome to my academic website</span>
    </div>

    
    <h1>An Yu Chen</h1>
    <p class="academic-subtitle">Academic Profile</p>
    <div class="academic-rule"></div>

    <p class="academic-intro">
     I am a researcher in science, technology and innovation policy. My research examines how scientific knowledge contributes to technological development and innovation, with a particular interest in green technologies, knowledge networks, and the links between academic research and industry. I use bibliometric and patent data, computational techniques, and mixed-methods approaches to investigate how knowledge is created, circulated, and translated into technological and societal outcomes. I hold a doctorate in Science, Technology and Innovation Policy from the University of Manchester, UK. I previously worked as a Postdoctoral Research Associate (PDRA) at the Manchester Institute of Innovation Research (MIoIR), where I conducted research on science, technology and innovation. I have also been a visiting researcher at the Entrepreneurship, Finance and Innovation (EFI) research group at Politecnico di Milano, Italy, and undertook a research internship at Otto von Guericke University Magdeburg, Germany. My academic and research experience has enabled me to develop an interdisciplinary perspective on the dynamics of innovation, the role of scientific knowledge in technological change, and the interactions between universities, industry, and wider innovation systems.
    </p>
  </section>

  <nav class="academic-actions" aria-label="Main profile links">
    <a href="{{ '/assets/CV.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer" class="academic-btn academic-btn-primary">View my CV ↗</a>
    <a href="{{ '/autobiography/' | relative_url }}" class="academic-btn academic-btn-secondary">About me →</a>
    <a href="#academic-research-interests" class="academic-btn academic-btn-secondary">Explore my research ↓</a>
  </nav>

  <!-- RESEARCH PROFILE -->
  <section class="academic-section" aria-labelledby="research-profile-heading">
    <div class="academic-highlight">
      <div class="academic-highlight-icon" aria-hidden="true">✦</div>
      <div class="academic-highlight-copy">
        <h2 id="research-profile-heading">Understanding how knowledge drives technological change</h2>
        <p>
          I study how scientific knowledge is sourced, exchanged, and translated into innovation. I am particularly interested in how technologies emerge and develop, how connections between science and industry shape innovation, and how research evidence can inform policy and support the transition towards a more sustainable economy.
        </p>
      </div>
    </div>
  </section>

  <!-- RESEARCH INTERESTS -->
  <section class="academic-section" id="academic-research-interests">
    <h2 class="academic-section-title">Research interests</h2>
    <div class="academic-interest-grid">

      <article class="academic-interest">
        <div class="academic-interest-icon" aria-hidden="true">↗</div>
        <h3>Economics of innovation</h3>
        <p>Technological change, knowledge creation, innovation outcomes, and the emergence and development of new technologies and industries.</p>
      </article>

      <article class="academic-interest">
        <div class="academic-interest-icon" aria-hidden="true">◎</div>
        <h3>Science of science</h3>
        <p>Scientific knowledge sourcing, researcher mobility, knowledge networks, and the relationships between academic research and industry.</p>
      </article>

      <article class="academic-interest">
        <div class="academic-interest-icon" aria-hidden="true">♻</div>
        <h3>Green innovation and sustainability</h3>
        <p>Scientific contributions to green technologies, low-carbon innovation, and the knowledge dynamics underpinning sustainability transitions.</p>
      </article>

      <article class="academic-interest">
        <div class="academic-interest-icon" aria-hidden="true">⌘</div>
        <h3>Computational research methods</h3>
        <p>Bibliometrics, patent analysis, network analysis, text classification, topic modelling, and natural language processing for large-scale research data.</p>
      </article>

      <article class="academic-interest">
        <div class="academic-interest-icon" aria-hidden="true">AI</div>
        <h3>AI and digital transformation</h3>
        <p>Computational and intelligent technologies, their implications for scientific practice, and emerging questions for research and innovation.</p>
      </article>

      <article class="academic-interest">
        <div class="academic-interest-icon" aria-hidden="true">⌖</div>
        <h3>Science, technology and innovation policy</h3>
        <p>Research ecosystems, policy evaluation, and the use of evidence to inform decisions about science, technology, innovation, and sustainability.</p>
      </article>

    </div>
  </section>

  <!-- CAREER AND EDUCATION -->
  <section class="academic-section">
    <h2 class="academic-section-title">Academic journey</h2>
    <div class="academic-timeline">

      <article class="academic-timeline-item">
        <span class="academic-timeline-date">2026</span>
        Contributed to WIPO's <em>Women, Innovation and Impact</em> publication and research outputs on doctoral graduates' contributions to innovation.
        <br>
        <a href="https://www.wipo.int/publications/en/details.jsp?id=4879" target="_blank" rel="noopener noreferrer">Explore the WIPO publication ↗</a>
      </article>

      <article class="academic-timeline-item">
        <span class="academic-timeline-date">2025–2026</span>
        Postdoctoral Research Associate in Science of Science Studies, Alliance Manchester Business School, University of Manchester.
      </article>

      <article class="academic-timeline-item">
          <span class="academic-timeline-date">2021–2026</span>
          PhD in Science, Technology and Innovation Policy,
          University of Manchester. Thesis:
          <em>The contribution of scientific knowledge to green
          technology development: Three essays.</em>
          <img
            src="{{ '/assets/graduation_photo.jpg' | relative_url }}"
            class="academic-graduation-photo"
            alt="Graduation photo"
            loading="lazy"
          >
        </article>

      <article class="academic-timeline-item">
        <span class="academic-timeline-date">2017–2020</span>
        Research Assistant, National Taiwan University. Contributed to science and technology policy projects, bibliometric research, and patent analysis.
      </article>

      <article class="academic-timeline-item">
        <span class="academic-timeline-date">2015</span>
        MA in Technology Management and Business Administration, National Tsing Hua University, Taiwan.
      </article>

      <article class="academic-timeline-item">
        <span class="academic-timeline-date">2013</span>
        BSc in Economics, National Tsing Hua University, Taiwan.
      </article>

    </div>
  </section>

  <!-- METHODS -->
  <section class="academic-section">
    <h2 class="academic-section-title">Methods and research practice</h2>
    <div class="academic-card">
      <p>
        My research combines quantitative analysis with computational and qualitative approaches. I have worked with large-scale publication and patent datasets from sources including Scopus, OpenAlex, Web of Science, and patent databases, and have developed analytical workflows for research projects and policy-facing outputs.
      </p>
      <p>
        My technical experience includes Python, R, PySpark, SQL, Stata, and SAS. My methodological toolkit includes bibliometric analysis, network analysis, text classification, topic modelling, natural language processing, and transformer-based language models. I value rigorous research design, transparent methods, reproducible workflows, and clear communication of findings.
      </p>
      <p>
        I have also contributed to interdisciplinary research projects, supported research assistants, presented work at international conferences, and contributed to academic manuscripts and reports for research and policy audiences.
      </p>
    </div>
  </section>

  <!-- RESEARCH APPROACH -->
  <section class="academic-section">
    <h2 class="academic-section-title">How I approach research</h2>
    <div class="academic-card">
      <p>
        I am interested in research that connects perspectives across disciplines and brings empirical evidence to questions with wider economic and societal relevance. I see scientific knowledge not as an isolated output, but as part of a broader innovation process involving researchers, firms, institutions, and policy environments.
      </p>
      <p>
        This perspective motivates my interest in collaborative and interdisciplinary research, as well as in making research findings accessible to academic, policy, and wider stakeholder communities.
      </p>
    </div>
  </section>

  <!-- CONTACT -->
  <section class="academic-contact" id="academic-contact">
    <h2>Let's connect</h2>
    <p>
      I welcome opportunities for research collaboration, academic exchange, and discussion on science, technology, innovation, and sustainability.
    </p>
    <a
      class="academic-social"
      href="https://www.linkedin.com/in/an-yu-chen"
      target="_blank"
      rel="noopener noreferrer"
    >Connect on LinkedIn ↗</a>
  </section>

  <!-- ACADEMIC NETWORK -->
  <section class="academic-section">
    <h2 class="academic-section-title">Academic network and international experience</h2>
    <div
      id="academic-network-map"
      class="academic-map"
      role="region"
      aria-label="Map showing selected academic and professional locations"
    ></div>
    <p class="academic-map-note">
      The map highlights selected institutions and locations associated with my academic and professional experience. Select a marker to view its details.
    </p>
  </section>

</div>

<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
<script>
(function () {
  function initializeAcademicMap() {
    var el = document.getElementById("academic-network-map");

    if (!el || typeof L === "undefined" || el.dataset.initialized === "true") {
      return;
    }

    el.dataset.initialized = "true";

    var map = L.map(el, {
      scrollWheelZoom: false,
      zoomControl: true
    }).setView([35, 35], 2);

    L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
      attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap contributors</a>',
      maxZoom: 19
    }).addTo(map);

    var locations = [
      {
        coords: [53.4668, -2.2339],
        title: "University of Manchester",
        detail: "PhD and postdoctoral research"
      },
      {
        coords: [45.4781, 9.2266],
        title: "Milan, Italy",
        detail: "Academic and research connections"
      },
      {
        coords: [24.7873, 120.9915],
        title: "National Tsing Hua University, Taiwan",
        detail: "Undergraduate and master's studies"
      },
      {
        coords: [52.1205, 11.6276],
        title: "Magdeburg, Germany",
        detail: "Research internship and academic experience"
      },
      {
        coords: [31.2304, 121.4737],
        title: "Shanghai, China",
        detail: "Academic and professional connections"
      }
    ];

    locations.forEach(function (item) {
      L.marker(item.coords)
        .addTo(map)
        .bindPopup("<strong>" + item.title + "</strong><br>" + item.detail);
    });

    window.setTimeout(function () {
      map.invalidateSize();
    }, 150);
  }

  if (document.readyState === "loading") {
    document.addEventListener("DOMContentLoaded", initializeAcademicMap);
  } else {
    initializeAcademicMap();
  }
})();
</script>
