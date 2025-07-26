---
layout: default
title: "Home"
---

<style>
  /* General Body Styles */
  body {
    font-family: 'Roboto', sans-serif; /* Modern, readable font */
    margin: 0;
    line-height: 1.6;
    color: #333; /* Darker text for readability */
    background-color: #f4f7f6; /* Light, subtle background */
  }

  /* Headings */
  h1, h2 {
    font-family: 'Montserrat', sans-serif; /* Complementary, strong heading font */
    color: #2c3e50;
    margin-bottom: 20px;
  }

  h1 {
    font-size: 3.5rem;
    color: #2c3e50; /* Stronger color for main heading */
  }

  h2 {
    font-size: 2.5rem;
  }

  /* Section Styling */
  .section {
    padding: 60px 20px;
    text-align: center;
    max-width: 1000px;
    margin: 0 auto;
    box-sizing: border-box; /* Include padding in element's total width and height */
  }

  /* Specific Section Backgrounds and Colors */
  .hero-section {
    background: linear-gradient(135deg, #f8c1cc, #fbe7a1); /* Soft, inviting gradient */
    color: #2c3e50;
    padding: 80px 20px;
  }

  .research-impact-section {
    background-color: #eaf2f1; /* A light, calming background */
    color: #333;
  }

  .about-me-section {
    background-color: #ffffff; /* Clean white background */
    color: #333;
  }

  .journey-section {
    background-color: #fbe7a1; /* Your original accent color, used thoughtfully */
    color: #2c3e50;
  }

  /* Profile Picture */
  .profile-picture {
    width: 180px;
    height: 180px;
    border-radius: 50%;
    border: 5px solid white;
    box-shadow: 0 8px 15px rgba(0, 0, 0, 0.1); /* Soft shadow for depth */
    margin-bottom: 30px;
    object-fit: cover; /* Ensures image covers the area without distortion */
  }

  /* Paragraphs in sections */
  .section p {
    font-size: 1.15rem;
    max-width: 800px;
    margin: 0 auto 30px auto; /* Add some bottom margin to paragraphs */
    line-height: 1.7;
  }

  /* Button Styling */
  .button {
    display: inline-block; /* Allows padding and margin to be applied effectively */
    background-color: #402127; /* Darker, more sophisticated button color */
    color: white;
    border: none;
    padding: 12px 25px;
    font-size: 1.1rem;
    border-radius: 30px;
    cursor: pointer;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2); /* More pronounced shadow */
    margin-top: 20px;
    text-decoration: none; /* Remove underline from link */
    transition: background-color 0.3s ease, transform 0.2s ease; /* Smooth transition for hover effects */
  }

  .button:hover {
    background-color: #5a313b; /* Slightly lighter on hover */
    transform: translateY(-2px); /* Slight lift effect */
  }

  /* Social Icons */
  .social-icons {
    margin-top: 30px;
    display: flex; /* Use flexbox for alignment */
    justify-content: center; /* Center the icons */
    gap: 20px; /* Space between icons */
  }

  .social-icons img {
    width: 45px; /* Adjust size for better balance */
    height: 45px;
    transition: transform 0.2s ease;
  }

  .social-icons img:hover {
    transform: translateY(-3px); /* Hover effect for icons */
  }

  /* List Styling (Journey Section) */
  .journey-list {
    list-style-type: none;
    padding: 0;
    font-size: 1.1rem;
    line-height: 1.8;
    max-width: 800px;
    margin: 0 auto;
    color: #333;
    text-align: left; /* Align list items to the left */
  }

  .journey-list li {
    margin-bottom: 18px;
    padding-left: 25px; /* Space for a custom bullet */
    position: relative;
  }

  .journey-list li::before {
    content: '•'; /* Custom bullet point */
    color: #402127; /* Accent color for bullet */
    font-size: 1.5rem;
    position: absolute;
    left: 0;
    top: -3px; /* Adjust vertical alignment */
  }

  /* Responsive Adjustments */
  @media (max-width: 768px) {
    h1 {
      font-size: 2.5rem;
    }

    h2 {
      font-size: 2rem;
    }

    .section {
      padding: 40px 15px;
    }

    .profile-picture {
      width: 150px;
      height: 150px;
    }

    .social-icons img {
      width: 40px;
      height: 40px;
    }
  }

  @media (max-width: 480px) {
    h1 {
      font-size: 2rem;
    }

    h2 {
      font-size: 1.8rem;
    }

    .section p {
      font-size: 1rem;
    }

    .button {
      padding: 10px 20px;
      font-size: 1rem;
    }
  }
</style>

<div class="section hero-section">
  <img src="assets/profile_picture.jpg" alt="Profile Picture" class="profile-picture">
  <h1>Hello and Welcome!</h1>
  <p>
    I’m <b>An Yu Chen</b>, a doctoral researcher passionate about uncovering the intricate linkages between science and technology. My research explores how science contributes to green technologies, shaping a sustainable future. Let's dive into a world of ideas, innovation, and impact!
  </p>
  <a href="assets/anyu.pdf" target="_blank" class="button">
    View My CV
  </a>
  <div class="social-icons">
    <a href="https://www.linkedin.com/in/an-yu-chen-130146342/" target="_blank">
      <img src="assets/linkedin.png" alt="LinkedIn">
    </a>
    </div>
</div>

<div class="section research-impact-section">
  <h2>Research Interests</h2>
  <p>
    My research investigates the linkages between science and technology, with a focus on the scientific knowledge base in green technologies. Through this, I aim to explore knowledge flows across fields of science, contributing to science and technology policy discussions.
  </p>

  <h2>Impact</h2>
  <p>
    My work addresses whether science can drive the advancement of emerging technologies, shaping discussions on sustainability and policy while identifying new avenues for research.
  </p>
</div>

<div class="section about-me-section">
  <h2>A Little About Me</h2>
  <p>
    I’m a curious, enthusiastic thinker who loves connecting with people and exploring fresh perspectives. I bring energy and creativity into my work and collaborations, always eager to learn and grow.
  </p>
</div>

<div class="section journey-section">
  <h2>Highlights of My Journey</h2>
  <ul class="journey-list">
    <li>
      <strong>PhD in Science, Technology and Innovation Policy</strong> | Alliance Manchester Business School, The University of Manchester (2021-Present)
    </li>
    <li>
      <strong>MSc in Business Administration in Technology Management</strong> | National Tsing Hua University (2013-2015)
    </li>
    <li>
      <strong>Research Assistant</strong> | The University of Manchester (2023-2024)
    </li>
    <li>
      <strong>Teaching Assistant</strong> | Database Systems, The University of Manchester (2023)
    </li>
  </ul>
</div>
