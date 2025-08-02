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
    --button-color: #e67e22;
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
  }

  .profile-pic {
    width: 180px;
    height: 180px;
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
    font-size: 1.1rem;
    max-width: 800px;
    margin: 0 auto;
    line-height: 1.8;
  }

  .cv-button {
    display: inline-block;
    background-color: var(--button-color);
    color: white;
    padding: 12px 30px;
    font-size: 1.1rem;
    border-radius: 25px;
    text-decoration: none;
    font-weight: 600;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    transition: background-color 0.3s ease, transform 0.2s ease;
  }

  .cv-button:hover {
    background-color: #d35400;
    transform: translateY(-2px);
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
    color: var(--secondary-color);
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
    color: var(--secondary-color);
  }

  /* LinkedIn-specific styles to honor your request */
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
    width: 250px;
    height: auto;
    max-width: 100%;
    margin-top: 50px;
  }
</style>

<div class="hero-section">
  <img src="assets/profile_picture.jpg" alt="An Yu Chen Profile Picture" class="profile-pic">
  <h1>An Yu Chen</h1>
  <p class="subtitle">Doctoral Researcher | Research Associate</p>
  <p class="intro-text">
    Hello and welcome to my academic website! I'm a Doctoral Researcher and Research Associate at the <a href="https://www.manchester.ac.uk/research/institutes-centres/innovation-research-institute/" style="color: var(--link-color); text-decoration: none;">Manchester Institute of Innovation Research</a>, based in the Alliance Manchester Business School at The University of Manchester. My work focuses on the intricate linkages between science and technology, specifically how scientific knowledge contributes to the development of green technologies. Through rigorous analysis and policy engagement, I aim to create real-world impact.
  </p>
  <a href="assets/anyu.pdf" target="_blank" class="cv-button">
    View My CV
  </a>
</div>

<div class="section section-primary">
  <h2>Research Experience</h2>
  <div class="experience-item">
    <h3>Research Associate, MIOIR & AMBS</h3>
    <h4>The University of Manchester | Apr 2025-Present</h4>
    <ul>
      <li>Worked on an EPO funded project with bibliometric metadata and large-scale PhD thesis datasets.</li>
      <li>Utilised virtualised Linux environments on server to efficiently download and process terabytes of big data.</li>
      <li>Constructed complex datasets, linking PhD thesis data to publication data using data from Scopus and OpenAlex.</li>
      <li>Contributed to drafting detailed methodological reports and analysis strategies.</li>
    </ul>
  </div>
</div>

<div class="section section-accent">
  <h2>Highlights of My Journey</h2>
  <ul class="highlights-list">
    <li>
      <strong>PhD in Science, Technology and Innovation Policy</strong>
      Alliance Manchester Business School, The University of Manchester (2021-Present)
    </li>
    <li>
      <strong>MSc in Business Administration in Technology Management</strong>
      National Tsing Hua University (2013-2015)
    </li>
    <li>
      <strong>Research Assistant</strong>
      The University of Manchester (2023-2024)
    </li>
    <li>
      <strong>Teaching Assistant</strong>
      Database Systems, The University of Manchester (2023)
    </li>
  </ul>
</div>

<div class="section section-primary">
  <h2>Research Interests</h2>
  <p class="large">
    My research explores the relationship between science and technology, with a particular focus on the scientific foundations of green technologies. My goal is to understand knowledge flows across scientific fields and contribute to important policy discussions in science, technology, and innovation.
  </p>
</div>

<div class="section section-accent">
  <h2>About Me</h2>
  <p class="large">
    I am a curious and enthusiastic thinker who thrives on connecting with people and exploring fresh perspectives. I bring energy and creativity to my work and collaborations, and I'm always eager to learn and grow.
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
