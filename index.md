---
layout: default
title: "Home"
---

<style>
  :root {
    --primary-color: #2c3e50;
    --secondary-color: #f39c12;
    --background-light: #f7f9fb;
    --background-accent: #fdf6e3;
    --text-color: #34495e;
    --link-color: #3498db;
    --highlight-color: #e67e22;
  }

  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    color: var(--text-color);
    background-color: var(--background-light);
    line-height: 1.6;
    margin: 0;
  }

  .section {
    padding: 60px 20px;
    text-align: center;
  }

  .section-primary {
    background-color: white;
    color: var(--primary-color);
  }

  .section-accent {
    background-color: var(--background-accent);
    color: var(--primary-color);
  }

  .hero-section {
    padding: 80px 20px;
    background: linear-gradient(135deg, #fef0c7, #fde4eb);
    color: var(--primary-color);
    text-align: center;
    transition: all 0.3s ease;
  }

  .hero-section:hover {
    background: linear-gradient(135deg, #fde4eb, #fef0c7);
  }

  .profile-pic {
    width: 250px;
    height: 250px;
    border-radius: 50%;
    border: 4px solid white;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    margin-bottom: 25px;
    object-fit: cover;
  }

  h1 {
    font-size: 3rem;
    margin-bottom: 10px;
    font-weight: 700;
  }

  .subtitle {
    font-size: 1.5rem;
    color: #7f8c8d;
    font-weight: 400;
    margin-bottom: 30px;
  }

  .intro-text {
    max-width: 800px;
    margin: 0 auto 30px;
    font-size: 1.15rem;
    line-height: 1.8;
  }

  h2 {
    font-size: 2.2rem;
    margin-bottom: 25px;
    font-weight: 600;
  }

  p.large {
    font-size: 1.15rem;
    max-width: 800px;
    margin: 0 auto;
    line-height: 1.8;
  }

  .experience-item {
    max-width: 900px;
    margin: 0 auto 30px;
    padding: 30px;
    background: white;
    border-radius: 12px;
    text-align: left;
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.05);
  }

  .experience-item h3 {
    margin-top: 0;
    font-size: 1.5rem;
    color: var(--secondary-color);
  }

  .experience-item h4 {
    font-size: 1.2rem;
    color: #7f8c8d;
    margin-bottom: 15px;
  }

  .experience-item ul {
    margin: 0;
    padding-left: 20px;
    list-style: none;
  }

  .experience-item li {
    position: relative;
    padding-left: 25px;
    margin-bottom: 10px;
    line-height: 1.6;
  }

  .experience-item li::before {
    content: '•';
    position: absolute;
    left: 0;
    color: var(--highlight-color);
    font-size: 1.2rem;
    line-height: 1;
  }

  .highlights-list {
    list-style: none;
    padding: 0;
    margin: 0 auto;
    max-width: 800px;
    text-align: left;
  }

  .highlights-list li {
    background-color: white;
    margin-bottom: 15px;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
    transition: box-shadow 0.3s ease;
  }

  .highlights-list li:hover {
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
  }

  .highlights-list strong {
    display: block;
    font-size: 1.15rem;
    margin-bottom: 5px;
    color: var(--highlight-color);
  }

  .connect-section {
    padding: 40px 20px;
    text-align: center;
    background: var(--background-accent);
  }

  .connect-section h2 {
    margin-top: 0;
  }

  .linkedin-icon-container {
    margin-top: 20px;
  }

  .linkedin-icon-container img {
    width: 350px;
    max-width: 100%;
    height: auto;
    margin-top: 50px;
    transition: transform 0.3s ease;
  }

  .linkedin-icon-container img:hover {
    transform: scale(1.05);
  }
</style>

<div class="hero-section">
  <img src="assets/profile_picture.jpg" alt="An Yu Chen Profile Picture" class="profile-pic">
  <h1>An Yu Chen</h1>
  <p class="subtitle">Doctoral Researcher | Research Associate</p>
  <p class="intro-text">
    Welcome! I'm a researcher at the <a href="https://www.mioir.manchester.ac.uk" style="color: var(--link-color); text-decoration: none;">Manchester Institute of Innovation Research</a>, Alliance Manchester Business School. I explore how scientific knowledge drives sustainable technology and informs policy, with a focus on green technologies, AI, and societal impact. Here you can learn about my research, collaborations, and public engagement.
  </p>
</div>

<div class="section section-primary">
  <h2>Research Experience</h2>
  <div class="experience-item">
    <h3>Research Associate, MIOIR & AMBS</h3>
    <h4>The University of Manchester | Apr 2025-Present</h4>
    <ul>
      <li>Leading EPO-funded projects linking bibliometric and PhD thesis datasets to study knowledge flows.</li>
      <li>Utilising virtualised Linux servers and advanced Python, R, and PySpark pipelines to handle terabytes of data.</li>
      <li>Drafting detailed methodological reports and analytical strategies for policy-relevant insights.</li>
      <li>Engaging with stakeholders, including UKRI, Innovate UK, and the Innovation Research Caucus.</li>
    </ul>
  </div>
</div>

<div class="section section-accent">
  <h2>Highlights of My Academic Journey</h2>
  <ul class="highlights-list">
    <li><strong>PhD in Science, Technology and Innovation Policy</strong> Alliance Manchester Business School (2021-Present)</li>
    <li><strong>MSc in Business Administration – Technology Management</strong> National Tsing Hua University (2013-2015)</li>
    <li><strong>Research Assistant</strong> The University of Manchester (2023-2024)</li>
    <li><strong>Teaching Assistant – Database Systems</strong> The University of Manchester (2023)</li>
  </ul>
</div>

<div class="section section-primary">
  <h2>Research Interests</h2>
  <p class="large">
    My research focuses on the intersection of science, technology, and sustainability, investigating knowledge flows, gender differences, and the foundations of green technologies. I aim to deliver evidence-based insights to inform policy and societal transitions toward net-zero and inclusive innovation.
  </p>
</div>

<div class="section section-accent">
  <h2>About Me</h2>
  <p class="large">
    I am passionate about collaborative research, data-driven insights, and translating complex analyses into actionable outcomes. I enjoy connecting with people, exploring interdisciplinary perspectives, and contributing to impactful projects that bridge academia, policy, and society.
  </p>
</div>

<div class="connect-section">
  <h2>Connect with Me</h2>
  <div class="linkedin-icon-container">
    <a href="https://www.linkedin.com/in/an-yu-chen-130146342/" target="_blank">
      <img src="assets/linkedin.png" alt="LinkedIn">
    </a>
  </div>
</div>
