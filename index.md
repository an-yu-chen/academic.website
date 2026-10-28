---
layout: default
title: "Home"
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css">

<style>
:root{--ab:#073d7b;--am:#0756a5;--ay:#ffd633;--ap:#fff9e8;--ink:#17385d;--muted:#56708c;--line:#e1eaf3}
.academic-home{font-family:"DM Sans","Segoe UI",sans-serif;color:var(--ink);font-size:16px;line-height:1.75;-webkit-font-smoothing:antialiased}
.academic-home *{box-sizing:border-box}.academic-home a{color:var(--am);text-decoration:none}.academic-home a:hover{color:var(--ab)}
.academic-hero{position:relative;overflow:hidden;display:flex;flex-direction:column;align-items:center;text-align:center;gap:0;padding:clamp(42px,6vw,72px) 24px 42px;color:var(--ink);background:#fff}
.academic-hero:before{content:"";position:absolute;top:27px;left:calc(50% - 32px);width:64px;height:5px;border-radius:8px;background:var(--ay)}.academic-hero:after{content:"";position:absolute;right:max(calc((100% - 1000px)/2),22px);top:45px;width:14px;height:14px;border-radius:50%;background:var(--ay);pointer-events:none}
.academic-eyebrow{margin:30px 0 0;color:var(--am);font-size:.78rem;font-weight:800;letter-spacing:.14em;text-transform:uppercase}
.academic-hero h1{margin:12px 0 10px;color:var(--ab);font:800 clamp(2.4rem,5vw,4.1rem)/1.08 "Manrope",sans-serif;letter-spacing:-.045em}
.academic-subtitle{max-width:850px;margin:0;color:var(--am);font:600 clamp(1rem,2vw,1.18rem)/1.7 "Manrope",sans-serif}
.academic-rule{width:58px;height:5px;margin:20px auto 17px;border-radius:8px;background:var(--ay)}
.academic-intro{max-width:790px;margin:0 auto;color:var(--muted);line-height:1.9}
.academic-profile-wrap{position:relative;z-index:1;display:flex;flex-direction:column;align-items:center}
.academic-profile{display:block;width:clamp(175px,21vw,235px);height:clamp(175px,21vw,235px);aspect-ratio:1;object-fit:cover;object-position:center;border:5px solid #fff;border-radius:50%;outline:2px solid var(--line);box-shadow:0 12px 34px #073d7b18}
.academic-profile-caption{display:inline-block;margin-top:17px;padding:7px 14px;color:var(--ab);background:#fff8d9;border:1px solid #ffeb9a;border-radius:999px;font-size:.8rem;font-weight:800}
.academic-actions{display:flex;justify-content:center;flex-wrap:wrap;gap:13px;padding:25px 18px 5px}
.academic-btn{display:inline-flex;align-items:center;justify-content:center;min-height:46px;padding:11px 22px;border-radius:999px;font:800 .92rem "Manrope",sans-serif;border:2px solid var(--ab);transition:transform .2s,box-shadow .2s}
.academic-btn:hover{transform:translateY(-2px);box-shadow:0 10px 30px #073d7b14}
.academic-btn-primary{color:#fff!important;background:var(--ab)}.academic-btn-secondary{color:var(--ab)!important;background:#fff;border-color:var(--line)}.academic-btn-secondary:hover{background:var(--ap);border-color:var(--ay)}
.academic-section{width:min(100% - 44px,1160px);margin:0 auto;padding:42px 0}
.academic-section-title{display:flex;align-items:center;gap:14px;margin:0 0 22px;color:var(--ab);font:800 clamp(1.45rem,3vw,1.9rem)/1.3 "Manrope",sans-serif;letter-spacing:-.025em}
.academic-section-title:before{content:"";flex:0 0 45px;height:5px;border-radius:8px;background:var(--ay)}
.academic-highlight{display:grid;grid-template-columns:82px 1fr;gap:22px;align-items:center;background:var(--ap);border:1px solid #ffefb2;border-radius:16px;padding:clamp(22px,3vw,30px)}
.academic-highlight-icon{display:grid;place-items:center;width:70px;height:70px;border:2px solid var(--ab);border-radius:50%;background:#fff;color:var(--ab);font-size:32px;box-shadow:6px 6px 0 var(--ay)}
.academic-highlight-copy{border-left:3px solid var(--ay);padding-left:22px}.academic-highlight h2{margin:0 0 8px;color:var(--ab);font:800 1.3rem "Manrope",sans-serif}.academic-highlight p{margin:0}
.academic-interest-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:17px}
.academic-interest{padding:23px 22px;background:#fff;border:1px solid var(--line);border-radius:15px;box-shadow:0 5px 16px #1035680a;transition:transform .25s,border-color .25s,box-shadow .25s}
.academic-interest:hover{transform:translateY(-4px);border-color:#bfd4f0;box-shadow:0 10px 30px #073d7b14}
.academic-interest-icon{display:grid;place-items:center;width:46px;height:46px;margin-bottom:14px;border-radius:14px;background:var(--ay);color:var(--ab);font-size:22px;font-weight:800}
.academic-interest h3{margin:0 0 8px;color:var(--ab);font:800 1.04rem/1.4 "Manrope",sans-serif}.academic-interest p{margin:0;color:var(--muted);font-size:.92rem;line-height:1.7}
.academic-timeline{display:flex;gap:20px;overflow-x:auto;padding:28px 8px 24px;scroll-snap-type:x mandatory;scrollbar-width:thin;scrollbar-color:#b8cbea #f0f4fa}
.academic-timeline-item{flex:0 0 280px;padding:24px 22px;background:#fff;border:1px solid var(--line);border-top:4px solid var(--ab);border-radius:15px;box-shadow:0 5px 18px #1035680d;font-size:.92rem;line-height:1.75;scroll-snap-align:start}
.academic-timeline-item:nth-child(even){border-top-color:var(--ay)}.academic-timeline-date{display:block;margin-bottom:9px;color:var(--ab);font:800 1rem "Manrope",sans-serif}.academic-timeline-item:nth-child(even) .academic-timeline-date{color:#806000}.academic-timeline-item a{display:inline-block;margin-top:8px;font-weight:700}
.academic-card{padding:clamp(22px,3vw,34px);background:#fff;border:1px solid var(--line);border-radius:17px;box-shadow:0 5px 18px #1035680b}.academic-card p:last-child{margin-bottom:0}
.academic-contact{margin-top:10px;padding:42px 24px;text-align:center;background:linear-gradient(115deg,#f3f8ff,#fffdf5);border-block:1px solid var(--line)}
.academic-contact h2{margin:0 0 10px;color:var(--ab);font:800 1.8rem "Manrope",sans-serif}.academic-contact h2:after{content:"";display:block;width:55px;height:4px;margin:12px auto;border-radius:8px;background:var(--ay)}
.academic-contact p{color:var(--muted)}.academic-social{display:inline-block;margin-top:6px;padding:10px 18px;background:var(--ab);color:#fff!important;border-radius:999px;font-weight:800}.academic-social:hover{background:var(--am)}
.academic-map{height:360px;width:100%;border:1px solid var(--line);border-radius:16px;background:#eaf2ff;box-shadow:0 10px 30px #073d7b14;z-index:1}.academic-map-note{margin:10px 0 0;color:var(--muted);font-size:.82rem}
@media(max-width:800px){.academic-hero{padding-top:58px}.academic-hero:after{right:24px;top:30px}.academic-profile{width:175px;height:175px}.academic-interest-grid{grid-template-columns:repeat(2,minmax(0,1fr))}}
@media(max-width:540px){.academic-section{width:calc(100% - 32px);padding:30px 0}.academic-hero{padding:54px 22px 32px}.academic-profile{width:150px;height:150px}.academic-highlight{grid-template-columns:1fr;gap:16px}.academic-highlight-copy{padding-left:16px}.academic-interest-grid{grid-template-columns:1fr}.academic-timeline-item{flex-basis:250px}.academic-map{height:290px}}
@media(prefers-reduced-motion:reduce){.academic-home *,.academic-home *:before,.academic-home *:after{scroll-behavior:auto!important;transition-duration:.01ms!important}}
</style>

<div class="academic-home">
  <section class="academic-hero">
    <div class="academic-profile-wrap">
      <img src="{{ '/assets/profile_picture.jpg' | relative_url }}" class="academic-profile" alt="Profile photo of An Yu Chen">
      <span class="academic-profile-caption">Dr. Chen earned PhD degree from University of Manchester</span>
    </div>
    <p class="academic-eyebrow">Science · Innovation · Sustainability</p>
    <h1>An Yu Chen</h1>
    <p class="academic-subtitle">Innovation Economics · Science of Science · Green Technological Change</p>
    <div class="academic-rule"></div>
    <p class="academic-intro">I am a researcher in science, technology and innovation policy. My research examines how scientific knowledge contributes to technological development, with particular interest in green innovation, knowledge networks, and the relationship between research and industry. I use bibliometric and patent data, computational methods, and mixed-methods approaches to study innovation and sustainability transitions.</p>
  </section>

  <div class="academic-actions">
    <a href="{{ '/assets/CV.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer" class="academic-btn academic-btn-primary">View CV ↗</a>
    <a href="{{ '/autobiography/' | relative_url }}" class="academic-btn academic-btn-secondary">Autobiography →</a>
    <a href="#academic-research-interests" class="academic-btn academic-btn-secondary">Explore Research ↓</a>
  </div>

  <section class="academic-section">
    <div class="academic-highlight">
      <div class="academic-highlight-icon" aria-hidden="true">✦</div>
      <div class="academic-highlight-copy">
        <h2>Research at the intersection of science and technological change</h2>
        <p>My work explores how scientific knowledge is sourced, exchanged, and translated into innovation. I am especially interested in the processes through which technologies emerge and develop, and how research evidence can inform innovation policy and the transition towards a more sustainable economy.</p>
      </div>
    </div>
  </section>

  <section class="academic-section" id="academic-research-interests">
    <h2 class="academic-section-title">Research Interests</h2>
    <div class="academic-interest-grid">
      <article class="academic-interest"><div class="academic-interest-icon">↗</div><h3>Economics of Innovation</h3><p>Technological change, knowledge creation, innovation outcomes, and the dynamics of emerging technologies and industries.</p></article>
      <article class="academic-interest"><div class="academic-interest-icon">◎</div><h3>Science of Science</h3><p>Scientific knowledge sourcing, researcher mobility, knowledge networks, and relationships between academic research and industry.</p></article>
      <article class="academic-interest"><div class="academic-interest-icon">♻</div><h3>Green Innovation</h3><p>Scientific contributions to green technologies, sustainability transitions, and the development of low-carbon technologies.</p></article>
      <article class="academic-interest"><div class="academic-interest-icon">⌘</div><h3>Computational Research</h3><p>Bibliometrics, patent analysis, network analysis, natural language processing, and large-scale research datasets.</p></article>
      <article class="academic-interest"><div class="academic-interest-icon">AI</div><h3>AI and Digital Transformation</h3><p>Computational and intelligent technologies, changing scientific practice, and emerging questions for research and innovation.</p></article>
      <article class="academic-interest"><div class="academic-interest-icon">⌖</div><h3>Science and Technology Policy</h3><p>Research ecosystems, policy evaluation, and evidence that supports decisions about science, technology, and innovation.</p></article>
    </div>
  </section>

  <section class="academic-section">
    <h2 class="academic-section-title">Academic Milestones</h2>
    <div class="academic-timeline">
      <article class="academic-timeline-item"><span class="academic-timeline-date">2026</span>Contributed to WIPO’s <em>Women, Innovation and Impact</em> publication and research outputs on doctoral graduates’ contribution to innovation.<br><a href="https://www.wipo.int/publications/en/details.jsp?id=4879" target="_blank" rel="noopener noreferrer">View WIPO publication →</a></article>
      <article class="academic-timeline-item"><span class="academic-timeline-date">2025–2026</span>Postdoctoral Research Associate in Science of Science Studies, Alliance Manchester Business School, University of Manchester.</article>
      <article class="academic-timeline-item"><span class="academic-timeline-date">2021–2026</span>PhD in Science, Technology and Innovation Policy, University of Manchester. Thesis: <em>The contribution of scientific knowledge to green technology development: Three essays.</em></article>
      <article class="academic-timeline-item"><span class="academic-timeline-date">2017–2020</span>Research Assistant, National Taiwan University. Contributed to science and technology policy projects, bibliometric research, and patent analysis.</article>
      <article class="academic-timeline-item"><span class="academic-timeline-date">2015</span>MA in Technology Management and Business Administration, National Tsing Hua University, Taiwan.</article>
      <article class="academic-timeline-item"><span class="academic-timeline-date">2013</span>BSc in Economics, National Tsing Hua University, Taiwan.</article>
    </div>
  </section>

  <section class="academic-section">
    <h2 class="academic-section-title">Methods &amp; Research Practice</h2>
    <div class="academic-card">
      <p>My research combines quantitative analysis with computational and qualitative approaches. I have worked with large-scale publication and patent datasets from sources including Scopus, OpenAlex, Web of Science, and patent databases, and have developed analytical workflows for research projects and policy-facing outputs.</p>
      <p>My technical experience includes Python, R, PySpark, SQL, Stata, and SAS, alongside bibliometric analysis, network analysis, text classification, topic modelling, natural language processing, and transformer-based language models. I value reproducible workflows, careful research design, and clear communication of methods and findings.</p>
      <p>I have also contributed to interdisciplinary projects, supported research assistants, presented work at international conferences, and contributed to academic manuscripts and reports for research and policy audiences.</p>
    </div>
  </section>

  <section class="academic-contact" id="academic-contact">
    <h2>Connect with Me</h2>
    <p>For research enquiries, collaboration, or academic discussion, please get in touch.</p>
    <a class="academic-social" href="https://www.linkedin.com/in/an-yu-chen" target="_blank" rel="noopener noreferrer">Connect on LinkedIn ↗</a>
  </section>

  <section class="academic-section">
    <h2 class="academic-section-title">Academic Network &amp; Global Experience</h2>
    <div id="academic-network-map" class="academic-map" role="application" aria-label="Interactive map showing selected academic and professional locations"></div>
    <p class="academic-map-note">Map markers show selected institutions and locations associated with my academic and professional experience. Select a marker for details.</p>
  </section>
</div>

<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
<script>
(function () {
  function initializeAcademicMap() {
    var el = document.getElementById("academic-network-map");
    if (!el || typeof L === "undefined" || el.dataset.initialized === "true") return;
    el.dataset.initialized = "true";
    var map = L.map(el, { scrollWheelZoom: false, zoomControl: true }).setView([35, 35], 2);
    L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
      attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap contributors</a>',
      maxZoom: 19
    }).addTo(map);
    [
      {coords:[53.4668,-2.2339],title:"University of Manchester",detail:"PhD and research appointments"},
      {coords:[45.4781,9.2266],title:"Milan, Italy",detail:"Academic and research connections"},
      {coords:[24.7873,120.9915],title:"National Tsing Hua University, Taiwan",detail:"Undergraduate and master's studies"},
      {coords:[52.1205,11.6276],title:"Magdeburg, Germany",detail:"Research internship and academic experience"},
      {coords:[31.2304,121.4737],title:"Shanghai, China",detail:"Academic and professional connections"}
    ].forEach(function (item) {
      L.marker(item.coords).addTo(map).bindPopup("<strong>"+item.title+"</strong><br>"+item.detail);
    });
    window.setTimeout(function(){map.invalidateSize();},150);
  }
  if (document.readyState === "loading") document.addEventListener("DOMContentLoaded", initializeAcademicMap);
  else initializeAcademicMap();
})();
</script>
