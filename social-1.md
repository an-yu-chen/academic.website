---
layout: default
title: "Personal Journey"
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Source+Serif+4:wght@300;400;500&display=swap');

.journey-container {
  max-width: 960px;
  margin: 4rem auto;
  padding: 0 2rem;
  font-family: 'Source Serif 4', serif;
  color: #3b2a1f;
  line-height: 1.75;
  background-color: #fbf7f2;
}

/* Header */
.journey-header {
  background: linear-gradient(135deg, #efe4d8, #e3d2c2);
  padding: 3.5rem 2.5rem;
  border-radius: 20px;
  text-align: center;
  margin-bottom: 3.5rem;
  box-shadow: 0 12px 28px rgba(0, 0, 0, 0.08);
}

.journey-header h1 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 3rem;
  font-weight: 600;
  color: #5a3e2b;
  margin-bottom: 0.8rem;
}

.journey-header p {
  font-size: 1.2rem;
  color: #6b4a35;
  max-width: 720px;
  margin: 0 auto;
}

/* Sections */
.journey-section {
  background: #ffffff;
  border-radius: 18px;
  padding: 2.8rem 3rem;
  box-shadow: 0 10px 26px rgba(0, 0, 0, 0.06);
  margin-bottom: 3.5rem;
}

.journey-section h2 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 2.2rem;
  color: #5a3e2b;
  margin-bottom: 1.2rem;
  font-weight: 600;
}

.journey-section p {
  font-size: 1.08rem;
  margin-bottom: 1.6rem;
  color: #3f2e22;
}

/* Magazine-style pull quote */
.quote {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.6rem;
  font-style: italic;
  color: #5a3e2b;
  margin: 2.8rem auto;
  padding: 1.5rem 2rem;
  max-width: 700px;
  text-align: center;
  position: relative;
}

.quote::before {
  content: "“";
  font-size: 4rem;
  position: absolute;
  left: -0.5rem;
  top: -1.5rem;
  color: #e0cbb8;
}

.quote::after {
  content: "”";
  font-size: 4rem;
  position: absolute;
  right: -0.5rem;
  bottom: -1.8rem;
  color: #e0cbb8;
}

/* Images */
.image-frame {
  margin: 4rem 0;
  text-align: center;
}

.image-frame img {
  max-width: 100%;
  border-radius: 18px;
  box-shadow: 0 12px 30px rgba(0, 0, 0, 0.12);
}

.image-caption {
  font-size: 0.95rem;
  color: #6b4a35;
  margin-top: 0.8rem;
  font-style: italic;
}
</style>

<div class="journey-container">

  <div class="journey-header">
    <h1>My Life-Changing Journey in Tanzania</h1>
  </div>

  <div class="journey-section">
    <h2>A Transformative Experience</h2>

    <p>
      In the summer of 2014, I travelled to Tanzania — a journey that gently but
      firmly reminded me that we are all deeply connected. What I encountered there
      was not only a different place, but a different way of seeing.
    </p>

    <p>
      I took part in a three-month educational volunteer programme in Tanzania,
      Africa. At the time, it seemed like a simple idea — something that felt like
      a fun opportunity — but in reality, it became a life-changing experience that
      I still return to in memory.
    </p>

    <p>
      We were involved in raising computers and covering shipping fees to support
      the delivery of equipment to local schools. Once on site, we utilised computer
      classrooms, provided basic PC training, and shared ICT knowledge through
      structured sessions. The work was practical, but the meaning of it unfolded
      slowly over time.
    </p>

    <p>
      As far as I recall, I arrived thinking I was there to contribute something
      technical. Instead, I realised that what I encountered was far more human.
      The openness of the students and teachers, and their eagerness to learn,
      moved me in ways I had not anticipated. I left feeling renewed in my own
      outlook.
    </p>

    <p>
      As a volunteer, I helped with computer teaching, setting up classrooms, and
      participating in cultural exchange. Yet, while I arrived thinking I was there
      to give, I found myself receiving far more. The openness, generosity, and
      patience of the people I met quietly reshaped my understanding of community.
    </p>
  </div>

  <div class="journey-section">
    <h2>Lessons That Stayed With Me</h2>

    <p>
      There were days filled with laughter, singing, and moments of shared silence.
      In those moments, I learned the value of being present — of noticing rather
      than rushing, of listening rather than leading.
    </p>

    <p>
      I have always responded to work with curiosity and excitement, and that
      experience deepened this instinct. My joy comes from seeing how small acts
      of teaching and exchange can create positive change. At the heart of it all
      is the simple truth that learning is always mutual.
    </p>

    <p>
      This experience also taught me to appreciate what is often overlooked, to
      approach others with gentleness, and to carry gratitude into everyday life.
    </p>

    <div class="quote">
      Do your little bit of good where you are; it is those little bits of good
      put together that overwhelm the world.
    </div>

    <p>
      Those words by Desmond Tutu stayed with me and remain lodged in my mind even
      now. It makes a great difference when one realises that knowledge-sharing is
      never one-directional. What they were learning, and the hope that seeds were
      planted, remain part of a memory I treasure deeply.
    </p>
  </div>

  <div class="image-frame">
    <img src="{{ site.baseurl }}/assets/han.jpg" alt="Computer Teaching">
    <p class="image-caption">
      Teaching computer skills — learning far more in return.
    </p>
  </div>

  <div class="image-frame">
    <img src="{{ site.baseurl }}/assets/tan.jpg" alt="My Journey in Tanzania">
    <p class="image-caption">
      A quiet moment captured during my time in Tanzania.
    </p>
  </div>

</div>
