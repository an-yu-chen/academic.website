
---
layout: default
title: "Home"
---

<style>
:root {
  --primary: #1f3c88;
  --accent: #3fa9f5;
  --soft: #f8fbff;
  --warm: #fffaf2;
  --text: #243447;
  --muted: #6b7280;
  --line: #dbeafe;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  background: white;
  color: var(--text);
  line-height: 1.7;
}

.hero {
  padding: 80px 20px;
  background: linear-gradient(135deg, #ffffff, #f7fbff);
  text-align: center;
}

.profile-pic {
  width: 220px;
  height: 220px;
  border-radius: 50%;
  object-fit: cover;
  border: 5px solid white;
  box-shadow: 0 10px 30px rgba(0,0,0,0.08);
  margin-bottom: 25px;
}

h1 {
  font-size: 3rem;
  margin-bottom: 10px;
}

.subtitle {
  font-size: 1.3rem;
  color: var(--muted);
}

.section {
  max-width: 1100px;
  margin: auto;
  padding: 70px 20px;
}

.section-title {
  text-align: center;
  font-size: 2.2rem;
  margin-bottom: 40px;
}

.timeline {
  position: relative;
  margin: 50px auto;
  padding-left: 40px;
  border-left: 4px solid var(--accent);
}

.timeline-item {
  position: relative;
  margin-bottom: 50px;
  background: var(--soft);
  padding: 28px;
  border-radius: 14px;
  box-shadow: 0 6px 20px rgba(0,0,0,0.04);
}

.timeline-item::before {
  content: "";
  position: absolute;
  left: -52px;
  top: 30px;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  background: var(--accent);
}

.year {
  font-size: 1.1rem;
  font-weight: 700;
  color: var(--primary);
}

.role {
  font-size: 1.35rem;
  font-weight: 700;
  margin: 8px 0;
}

.place {
  color: var(--muted);
  margin-bottom: 12px;
}

.quick-links {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(220px,1fr));
  gap: 20px;
  margin-top: 30px;
}

.card {
  background: white;
  border: 1px solid #eef2ff;
  border-radius: 16px;
  padding: 28px;
  text-align: center;
  box-shadow: 0 8px 24px rgba(0,0,0,0.04);
}

.card a {
  text-decoration: none;
  color: var(--primary);
  font-weight: 600;
}

.contact-box {
  background: var(--warm);
  border-radius: 18px;
  padding: 40px;
  text-align: center;
}
</style>

<div class="hero">
  <img src="/assets/profile.jpg" alt="An Yu Chen" class="profile-pic">
  <h1>An Yu Chen</h1>
  <p class="subtitle">Research Associate in Science of Science | University of Manchester</p>

  <p>
    Manchester Institute of Innovation Research (MIOIR) & Alliance Manchester Business School (AMBS)<br>
    Booth Street West, Manchester, UK, M15 6PB<br>
    +44 (0)7787872338 | chen.an.yu@outlook.com
  </p>
</div>

<div class="section">
  <h2 class="section-title">Academic Milestone Timeline (2015–2025)</h2>

  <div class="timeline">

    <div class="timeline-item">
      <div class="year">2025 – Present</div>
      <div class="role">Research Associate in Science of Science</div>
      <div class="place">MIOIR & AMBS, The University of Manchester</div>
      <p>EPO-funded project using Scopus, OpenAlex and large-scale PhD thesis datasets. Big-data analysis using Linux servers, Python, R and bibliometric methods. Policy engagement with UKRI and Innovation Research Caucus.</p>
    </div>

    <div class="timeline-item">
      <div class="year">March 2025</div>
      <div class="role">Visiting Scholar</div>
      <div class="place">Politecnico di Milano</div>
      <p>Research seminar with EFI community on scientific knowledge and technology development. Supported international PhD collaboration between Polimi and AMBS.</p>
    </div>

    <div class="timeline-item">
      <div class="year">2024</div>
      <div class="role">Research Assistant – UK Doctoral Graduates Project</div>
      <div class="place">University of Manchester</div>
      <p>Worked on UK Doctrack project with bibliometric data, text mining verification, gender and ethnicity analysis, and technical reports using R and Python.</p>
    </div>

    <div class="timeline-item">
      <div class="year">2023–2024</div>
      <div class="role">Research Assistant – Multiple Affiliations Project</div>
      <div class="place">University of Manchester</div>
      <p>Used PySpark and topic modelling on Scopus publication data. Explored simultaneous academia–industry affiliations and AI-related research outputs.</p>
    </div>

    <div class="timeline-item">
      <div class="year">2023</div>
      <div class="role">Teaching Assistant – Database Systems</div>
      <div class="place">Computer Science Department, University of Manchester</div>
      <p>Supported undergraduate database systems teaching, assignment marking and lab sessions with students.</p>
    </div>

    <div class="timeline-item">
      <div class="year">2021–2025</div>
      <div class="role">PhD in Science, Technology and Innovation Policy</div>
      <div class="place">Alliance Manchester Business School</div>
      <p>Thesis: <em>The Contribution of Scientific Knowledge to Green Technology Development: Three Essays</em>. Viva passed July 23rd, 2025.</p>
    </div>

    <div class="timeline-item">
      <div class="year">2017–2020</div>
      <div class="role">Student Research Assistant</div>
      <div class="place">National Taiwan University</div>
      <p>Publication analysis, management research support, and academic journal assistance.</p>
    </div>

    <div class="timeline-item">
      <div class="year">2016–2017</div>
      <div class="role">Customer Service Specialist</div>
      <div class="place">Booking.com</div>
      <p>XML system management and international customer support in multicultural operations.</p>
    </div>

    <div class="timeline-item">
      <div class="year">2013–2015</div>
      <div class="role">MA in Business Administration (Technology Management)</div>
      <div class="place">National Tsing Hua University</div>
      <p>Developed strong foundations in technology management, innovation and strategic research.</p>
    </div>

  </div>
</div>

<div class="section">
  <h2 class="section-title">Explore My Academic Work</h2>

  <div class="quick-links">
    <div class="card"><a href="/research/">Research</a><p>Projects, papers, publications, working papers and conferences</p></div>
    <div class="card"><a href="/teaching/">Teaching</a><p>Teaching assistantship, student support and reflections</p></div>
    <div class="card"><a href="/social-responsibility/">Social Responsibility</a><p>Policy engagement, mentoring and public contribution</p></div>
    <div class="card"><a href="/contact/">Contact</a><p>Collaboration opportunities and academic partnerships</p></div>
  </div>
</div>

<div class="section">
  <div class="contact-box">
    <h2>Contact</h2>
    <p>
      I welcome collaboration opportunities, research visits, seminars and joint academic projects.<br><br>
      <strong>Email:</strong> chen.an.yu@outlook.com<br>
      <strong>Phone:</strong> +44 (0)7787872338
    </p>
  </div>
</div>
 

 
