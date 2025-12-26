---
layout: default
title: "Biography"
---
<style>
    :root {
        /* Light mode colors */
        --bg-color-primary: #e3f2fd;
        --bg-color-secondary: #fefefe;
        --text-color-primary: #1a237e;
        --text-color-secondary: #37474f;
        --link-color: #1565c0;
    }

    /* Dark mode colors */
    @media (prefers-color-scheme: dark) {
        :root {
            --bg-color-primary: #1c1c1c;
            --bg-color-secondary: #2c2c2c;
            --text-color-primary: #e0e0e0;
            --text-color-secondary: #bdbdbd;
            --link-color: #64b5f6;
        }
    }

    body {
        margin: 0;
        font-family: 'Segoe UI', 'Roboto', sans-serif;
        background-color: var(--bg-color-secondary);
        color: var(--text-color-secondary);
        padding: 0 20px;
    }

    .header-section {
        text-align: center;
        padding: 60px 20px;
        background-color: var(--bg-color-primary);
        color: var(--text-color-primary);
    }

    .header-section h1 {
        font-size: 3rem;
        font-weight: bold;
        color: var(--text-color-primary);
    }

    .content-section {
        max-width: 900px;
        margin: 40px auto;
        padding: 0 20px;
    }

    .content-section h2 {
        color: var(--text-color-primary);
        margin-top: 40px;
    }

    .content-section a {
        color: var(--link-color);
    }

    .content-section p {
        line-height: 1.8;
    }
</style>

<div class="header-section">
    <h1>Biography</h1>
    <p style="font-size: 1.2rem; max-width: 850px; margin: 0 auto; line-height: 1.7;">
    </p>
</div>

<div class="content-section">
    <h2>PhD Research</h2>
    <p>
        My research interests lie in understanding how scientific knowledge is created, recombined, and translated into technological innovation, and how this process affects the ways societies address large-scale challenges such as climate change and sustainability. This interest was piqued during my PhD research and continues to grow within my current work, where I attempt to address the challenges associated with mobilising scientific knowledge for socially impactful innovation. I am particularly interested in questions such as: What kinds of scientific knowledge matter most for technological impact? How do diversity, interdisciplinarity, and novelty shape innovation outcomes? And how can policy better support the translation of science into sustainable technologies?
    </p>
    <p>
        My doctoral research at the University of Manchester focused on the dynamic relationship between scientific knowledge and technological innovation, particularly within the field of green technologies. A significant part of my work involved linking green patent data with scientific publication data to explore how knowledge from science contributes to emerging technologies. Across three papers, I analysed different aspects of this linkage. The first examines how the extent of scientific citations in patents correlates with their generality and future citation impact. The second investigates how various types of knowledge recombination—such as interdisciplinary and atypical scientific combinations—affect technological outcomes. The third brings in a socio-technical lens, examining how gender homophily among inventors influences the selection of scientific publications cited in green patents.
    </p>
    <p>
        This work contributes to understanding how research and diversity in scientific practices can shape the future of green technology development. I set up a research plan from scratch, including the initial coding of large-scale patent and publication datasets, data cleaning, and the development of a statistically robust analysis strategy using Python and The R Project for Statistical Computing. I have applied topic modelling, text mining, and network analysis to understand patterns in scientific publications and patents. 
    </p>
    <p>
        I successfully secured additional PhD funding, independently managed my PhD budget and resources, and translated complex research findings into clear written reports and oral presentations for both specialist and non-specialist audiences.
    </p>

    <h2>Current Role: Research Associate</h2>
    <p>
        I worked as a research associate for Prof. Cornelia Lawson and Dr. Xin Deng, where we were building a UK doctoral graduate database. I am interested in exploring how research and science in the UK translate into technological practices and applications (please see:
        <a href="https://www.mioir.manchester.ac.uk/research/projects/uk-dgci/">UK DGCI</a>) Our work involves building a longitudinal database of UK doctoral graduates to explore career trajectories, mobility, and contributions to academia and industry. As such, this project has provided important data which will be used to inform innovation and research policy discussions in the UK and beyond. My work involves building data infrastructures and analytics pipelines for large, multi-source datasets, including bibliometric metadata from Scopus, OpenAlex, and large-scale doctoral thesis databases. This role allows me to apply my skills in data architecture, API integration, and policy-focused research design. I also think that I’ve been serving as a role of data scientist in a technology development and delivery capacity, I support work in multidisciplinary teams and advanced AI-driven research practices. More than that, this work required resilience and persistence, this meant that I’ve been training myself and picking myself up when I stumbled, and trying another way forward. Through this process, I developed the ability to make a tangible impact by offering innovative ideas and practical solutions grounded in rigorous data analysis.
    </p>

    <h2>Programming & Analytical Skills</h2>
    <p>
        I work primarily in <strong>Python</strong> and <strong>R</strong> for tasks like data collection, processing, visualization, and modeling. Early in my PhD, I used the Bibliometrix R package to map citation networks, then adopted <code>pybliometrics</code> to retrieve Scopus data via APIs. My core Python stack includes <code>numpy</code>, <code>pandas</code>, <code>scipy</code>, <code>matplotlib</code>, and <code>statsmodels</code>. In R, I frequently use <code>dplyr</code> and <code>ggplot2</code> for data wrangling and visualization. Later in my researcher role, I have developed even more stronger programming experience in Python and R, and extensive experience with relevant analytics libraries such as <code>linearmodels</code>, <code>PyTorch</code>, and <code>scikit-learn</code>. I regularly work with large datasets, virtualised Linux environments, and cloud or server-based infrastructures to process terabytes of data efficiently. I actively continue to expand my expertise in AI and machine learning models and pipelines.
    </p>
    <p>
        I’ve taken part in advanced training through <a href="https://www.risis2.eu/">RISIS</a> data workshops, the AI4STIP Winter School (focused on LLMs and NLP), and Andrew Ng’s machine learning course. I also work in a Linux virtual environment to manage data pipelines and metadata infrastructures. Approximately 68% of my current work could be classified as applied data science.
    </p>
    <p>
        I thrive in a high-performance, high-reward culture. My transferable skills include strong communication through regular oral presentations at seminars and conferences; teamwork through developing links with colleagues, collaborators, and interns; and organisation through conference volunteering and managing complex, deadline-driven projects alongside teaching and research commitments.
    </p>

    <h2>Teaching Experience</h2>
    <p>
        During my doctoral training, I gained hands-on teaching experience at the University of Manchester, supporting undergraduate courses in the Department of Computer Science. As a Teaching Assistant for “Database Systems,” I led lab tutorials and provided project support to students working on relational database design and queries.
    </p>
    <p>
        I completed the <strong>AMBS TA Professional Development Workshop Series</strong>, which trained me in key teaching techniques—ranging from public speaking and the use of graphical aids to fostering classroom interaction and providing constructive feedback. I also explored strategies for supporting international students and reflecting on my TA experience to strengthen academic job applications.
    </p>
    <p>
        To improve student engagement, I incorporate digital tools like <strong>Mentimeter</strong>, <strong>Padlet</strong>, <strong>Slido</strong>, and <strong>Poll Everywhere</strong>. These platforms help me create inclusive, interactive sessions that respond to student feedback in real time.
    </p>

    <h2>Looking Ahead</h2>
    <p>
        I aim to continue laying a pivotal role in interdisciplinary research that bridges science, data, and technology. More precisely, my long-term aim is to contribute to high-impact, interdisciplinary research that informs innovation policy and addresses pressing societal challenges. I hope to expand my research into the roles of science and diversity in shaping responsible technologies, continue mentoring students, and contribute to collaborative, international research communities.
    </p>
</div>
