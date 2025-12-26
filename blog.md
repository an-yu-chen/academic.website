---
layout: default
title: "Biography"
---
<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700&family=Lora:wght@400;700&display=swap');

.bio-container {
  max-width: 900px;
  margin: 2rem auto;
  padding: 0 2rem;
  font-family: 'Lora', serif;
  color: #333; /* main text dark grey */
  line-height: 1.8;
  background-color: #fcf8f1; /* cream page background */
}

/* Bio Header */
.bio-header {
  background: linear-gradient(145deg, #fff8f0, #ffeedd);
  padding: 3rem 2rem;
  border-radius: 20px;
  text-align: center;
  margin-bottom: 3rem;
  box-shadow: 0 15px 35px rgba(0, 0, 0, 0.08);
}

.bio-header h1 {
  font-family: 'Merriweather', serif;
  font-size: 3rem;
  color: #e07a5f; /* warm coral */
  margin-bottom: 0.5rem;
  letter-spacing: 1px;
}

.bio-header p {
  font-size: 1.35rem;
  color: #555; /* soft dark grey */
  max-width: 700px;
  margin: 0 auto;
  line-height: 1.6;
  font-style: italic;
}

/* Bio Sections */
.bio-section {
  background: #ffffff; /* white for text areas */
  border-radius: 20px;
  padding: 3rem;
  box-shadow: 0 12px 30px rgba(0, 0, 0, 0.07);
  margin-bottom: 3rem;
  transition: transform 0.3s ease;
}
.bio-section:hover {
  transform: translateY(-2px);
}

.bio-section h2 {
  font-family: 'Merriweather', serif;
  font-size: 2.2rem;
  color: #333; /* dark grey for headings */
  margin-bottom: 1.5rem;
  font-weight: 700;
  border-bottom: 2px solid #ffeedd;
  padding-bottom: 0.5rem;
}

.bio-section p {
  font-size: 1.17rem;
  margin-bottom: 1.8rem;
  color: #333; /* main text dark grey */
}

/* Pull Quote Style */
.pull-quote {
  font-family: 'Merriweather', serif;
  font-style: italic;
  font-size: 1.35rem;
  color: #f4a261; /* orange accent */
  border-left: 6px solid #e9c46a; /* yellow accent */
  padding-left: 1.5rem;
  margin: 2.5rem 0;
  max-width: 800px;
  text-align: center;
  position: relative;
  background-color: #fffefb;
  border-radius: 10px;
}

.pull-quote::before {
  content: "“";
  font-size: 4.5rem;
  position: absolute;
  left: -0.6rem;
  top: -1.2rem;
  color: #ffe8c2;
}

.pull-quote::after {
  content: "”";
  font-size: 4.5rem;
  position: absolute;
  right: -0.6rem;
  bottom: -1.2rem;
  color: #ffe8c2;
}

/* Image Styling */
.image-frame {
  margin: 3rem 0;
  text-align: center;
}

.image-frame img {
  max-width: 100%;
  border-radius: 20px;
  box-shadow: 0 15px 35px rgba(0, 0, 0, 0.12);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.image-frame img:hover {
  transform: scale(1.03);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
}

.image-caption {
  font-size: 1rem;
  color: #9a8c98; /* soft purple-gray */
  margin-top: 0.8rem;
  font-style: italic;
  text-align: center;
}

/* Links (optional accent) */
a {
  color: #e07a5f; /* coral */
  text-decoration: underline;
}
a:hover {
  color: #f4a261; /* orange accent */
  text-decoration: none;
}
</style>



<div class="bio-container">

  <div class="bio-header">
    <h1>Biography</h1>
    <p>A journey bridging research, data, and innovation, with a focus on impactful interdisciplinary projects.</p>
  </div>

  <div class="bio-section">
    <h2>PhD Research</h2>
    <p>My research interests lie in understanding how scientific knowledge is created, recombined, and translated into technological innovation, and how this process affects the ways societies address large-scale challenges such as climate change and sustainability. This interest was piqued during my PhD research and continues to grow within my current work, where I attempt to address the challenges associated with mobilising scientific knowledge for socially impactful innovation. I am particularly interested in questions such as: What kinds of scientific knowledge matter most for technological impact? How do diversity, interdisciplinarity, and novelty shape innovation outcomes? And how can policy better support the translation of science into sustainable technologies?</p>

    <p>My doctoral research at the University of Manchester focused on the dynamic relationship between scientific knowledge and technological innovation, particularly within the field of green technologies. A significant part of my work involved linking green patent data with scientific publication data to explore how knowledge from science contributes to emerging technologies. Across three papers, I analysed different aspects of this linkage. The first examines how the extent of scientific citations in patents correlates with their generality and future citation impact. The second investigates how various types of knowledge recombination—such as interdisciplinary and atypical scientific combinations—affect technological outcomes. The third brings in a socio-technical lens, examining how gender homophily among inventors influences the selection of scientific publications cited in green patents.</p>

    <p>This work contributes to understanding how research and diversity in scientific practices can shape the future of green technology development. I set up a research plan from scratch, including the initial coding of large-scale patent and publication datasets, data cleaning, and the development of a statistically robust analysis strategy using Python and The R Project for Statistical Computing. I have applied topic modelling, text mining, and network analysis to understand patterns in scientific publications and patents.</p>

    <p>I successfully secured additional PhD funding, independently managed my PhD budget and resources, and translated complex research findings into clear written reports and oral presentations for both specialist and non-specialist audiences.</p>
  </div>

  <div class="bio-section">
    <h2>Current Role: Research Associate</h2>
    <p>I worked as a research associate for Prof. Cornelia Lawson and Dr. Xin Deng, where we were building a UK doctoral graduate database. I am interested in exploring how research and science in the UK translate into technological practices and applications (please see: UK DGCI). Our work involves building a longitudinal database of UK doctoral graduates to explore career trajectories, mobility, and contributions to academia and industry. As such, this project has provided important data which will be used to inform innovation and research policy discussions in the UK and beyond.</p>

    <p>My work involves building data infrastructures and analytics pipelines for large, multi-source datasets, including bibliometric metadata from Scopus, OpenAlex, and large-scale doctoral thesis databases. This role allows me to apply my skills in data architecture, API integration, and policy-focused research design. I also think that I’ve been serving as a role of data scientist in a technology development and delivery capacity, I support work in multidisciplinary teams and advanced AI-driven research practices. More than that, this work required resilience and persistence, this meant that I’ve been training myself and picking myself up when I stumbled, and trying another way forward. Through this process, I developed the ability to make a tangible impact by offering innovative ideas and practical solutions grounded in rigorous data analysis.</p>
  </div>

  <div class="bio-section">
    <h2>Programming & Analytical Skills</h2>
    <p>I work primarily in Python and R for tasks like data collection, processing, visualization, and modeling. Early in my PhD, I used the Bibliometrix R package to map citation networks, then adopted pybliometrics to retrieve Scopus data via APIs. My core Python stack includes numpy, pandas, scipy, matplotlib, and statsmodels. In R, I frequently use dplyr and ggplot2 for data wrangling and visualization. Later in my researcher role, I have developed even more stronger programming experience in Python and R, and extensive experience with relevant analytics libraries such as linearmodels, PyTorch, and scikit-learn. I regularly work with large datasets, virtualised Linux environments, and cloud or server-based infrastructures to process terabytes of data efficiently. I actively continue to expand my expertise in AI and machine learning models and pipelines.</p>

    <p>I’ve taken part in advanced training through RISIS data workshops, the AI4STIP Winter School (focused on LLMs and NLP), and Andrew Ng’s machine learning course. I also work in a Linux virtual environment to manage data pipelines and metadata infrastructures. Approximately 68% of my current work could be classified as applied data science.</p>

    <p>I thrive in a high-performance, high-reward culture. My transferable skills include strong communication through regular oral presentations at seminars and conferences; teamwork through developing links with colleagues, collaborators, and interns; and organisation through conference volunteering and managing complex, deadline-driven projects alongside teaching and research commitments.</p>
  </div>

  <div class="bio-section">
    <h2>Teaching Experience</h2>
    <p>During my doctoral training, I gained hands-on teaching experience at the University of Manchester, supporting undergraduate courses in the Department of Computer Science. As a Teaching Assistant for Database Systems, I led lab tutorials and provided project support to students working on relational database design and queries.</p>

    <p>I completed the AMBS TA Professional Development Workshop Series, which trained me in key teaching techniques—ranging from public speaking and the use of graphical aids to fostering classroom interaction and providing constructive feedback. I also explored strategies for supporting international students and reflecting on my TA experience to strengthen academic job applications.</p>

    <p>To improve student engagement, I incorporate digital tools like Mentimeter, Padlet, Slido, and Poll Everywhere. These platforms help me create inclusive, interactive sessions that respond to student feedback in real time.</p>
  </div>

  <div class="bio-section">
    <h2>Looking Ahead</h2>
    <p>I aim to continue laying a pivotal role in interdisciplinary research that bridges science, data, and technology. More precisely, my long-term aim is to contribute to high-impact, interdisciplinary research that informs innovation policy and addresses pressing societal challenges. I hope to expand my research into the roles of science and diversity in shaping responsible technologies, continue mentoring students, and contribute to collaborative, international research communities.</p>
  </div>

</div>
