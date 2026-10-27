---
layout: archive
title: "Academic CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

<style>
  /* Match the Outreach & Media page, while keeping the CV easy to scan. */
  .academic-cv {
    --cv-accent: #97a2cf;
    --cv-link: #586a9e;
    --cv-text: #414654;
    --cv-muted: #667085;
    --cv-tint: #f5f6fc;
    --cv-border: #e7e9f2;
    color: var(--cv-text);
    container: academic-cv / inline-size;
  }

  .academic-cv * { box-sizing: border-box; }
  .academic-cv a { color: var(--cv-link); }
  .academic-cv a:hover { text-decoration: underline; }
  .academic-cv a:focus-visible { outline: 3px solid var(--cv-accent); outline-offset: 3px; }
  .academic-cv p { margin-top: 0; line-height: 1.55; }

  .academic-cv .cv-intro {
    margin: .15rem 0 1.05rem;
    font-size: .94rem;
  }
  .academic-cv .cv-button {
    display: inline-block;
    padding: .68rem .9rem;
    border: 1px solid #6b79aa;
    border-radius: 6px;
    background: #6b79aa;
    color: #fff;
    font-size: .83rem;
    font-weight: 650;
    line-height: 1.3;
    text-decoration: none;
  }
  .academic-cv .cv-button:hover {
    background: #526291;
    border-color: #526291;
    color: #fff;
    text-decoration: none;
  }

  /* A single featured appointment, like the BBC highlight on Outreach. */
  .academic-cv .cv-feature {
    margin: .25rem 0 2.15rem;
    padding: clamp(.9rem, 2vw, 1.4rem);
    border: 1px solid var(--cv-border);
    border-top: 4px solid var(--cv-accent);
    border-radius: 12px;
    background: var(--cv-tint);
  }
  .academic-cv .cv-eyebrow {
    display: block;
    margin: 0 0 .45rem;
    color: var(--cv-link);
    font-size: .7rem;
    font-weight: 750;
    letter-spacing: .09em;
    text-transform: uppercase;
  }
  .academic-cv .cv-feature h2 {
    margin: 0 0 .5rem;
    font-size: clamp(1.23rem, 2.5vw, 1.55rem);
    line-height: 1.27;
  }
  .academic-cv .cv-feature p { margin: 0 0 .25rem; font-size: .91rem; }
  .academic-cv .cv-feature .cv-date { margin: .7rem 0 0; }

  .academic-cv .cv-section { margin: 0 0 2.15rem; }
  .academic-cv .cv-section-title {
    margin: 0 0 .9rem;
    font-size: 1.4rem;
    line-height: 1.3;
  }
  .academic-cv .cv-date {
    color: var(--cv-link);
    font-size: .78rem;
    font-weight: 700;
    letter-spacing: .01em;
  }
  .academic-cv .cv-institution {
    margin-bottom: .65rem;
    color: var(--cv-muted);
    font-size: .87rem;
  }

  /* Education: three compact cards at wider article sizes. */
  .academic-cv .cv-education {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: .9rem;
  }
  .academic-cv .cv-education .cv-entry {
    display: flex;
    flex-direction: column;
  }
  .academic-cv .cv-education details {
    margin-top: auto;
    padding-top: .45rem;
    font-size: .81rem;
    border-top: 1px solid var(--cv-border);
  }
  .academic-cv .cv-education summary { color: var(--cv-link); cursor: pointer; font-weight: 650; }
  .academic-cv .cv-education details p { margin: .5rem 0 0; }
  .academic-cv .cv-paper-status { color: var(--cv-link); font-size: .78rem; font-style: italic; }
  .academic-cv .cv-actions { display: flex; gap: .65rem; flex-wrap: wrap; margin: 0 0 1.4rem; }
  .academic-cv .cv-button-secondary { background: #fff; color: var(--cv-link); border-color: var(--cv-accent); }
  .academic-cv .cv-button-secondary:hover { color: #fff; }

  .academic-cv .cv-entry {
    min-width: 0;
    padding: 1rem 1.15rem;
    border: 1px solid var(--cv-border);
    border-radius: 10px;
    background: #fff;
  }
  .academic-cv .cv-entry h3 {
    margin: 0 0 .3rem;
    font-size: 1.05rem;
    line-height: 1.35;
  }
  .academic-cv .cv-entry p { margin-bottom: .4rem; font-size: .86rem; }
  .academic-cv .cv-entry p:last-child { margin-bottom: 0; }
  .academic-cv .cv-entry .cv-date { margin: 0 0 .6rem; }
  .academic-cv .cv-meta {
    padding-top: .5rem;
    border-top: 1px solid var(--cv-border);
  }
  .academic-cv .cv-meta strong { font-weight: 650; }

  /* Earlier research: lighter two-card layout, as on Outreach. */
  .academic-cv .cv-research-grid {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: .95rem;
  }
  .academic-cv .cv-research-grid .cv-entry {
    border-top: 3px solid var(--cv-accent);
  }
  .academic-cv .cv-research-grid .cv-entry h3 { margin-bottom: .3rem; }
  .academic-cv .cv-research-grid .cv-role {
    margin-bottom: .2rem;
    font-weight: 650;
  }
  .academic-cv .cv-research-grid .cv-date { margin-bottom: .65rem; }

  /* Breakpoints follow the article width (the theme also has a sidebar). */
  @container academic-cv (min-width: 650px) {
    .academic-cv .cv-education { grid-template-columns: repeat(3, minmax(0, 1fr)); }
    .academic-cv .cv-education .cv-entry { padding: .85rem; }
    .academic-cv .cv-education .cv-entry h3 { font-size: .96rem; }
  }
  @container academic-cv (min-width: 560px) {
    .academic-cv .cv-research-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  }
  @container academic-cv (max-width: 430px) {
    .academic-cv .cv-entry { padding: .85rem .9rem; }
  }
</style>

<div class="academic-cv">

  <p class="cv-intro">
    A quick overview of my academic background. For publications, talks and other details, you can find my full CV below.
  </p>
  <div class="cv-actions">
    <a class="cv-button" href="https://fvandonkelaar.github.io/files/CV.pdf" target="_blank" rel="noopener noreferrer">Full CV (PDF) &rarr;</a>
    <a class="cv-button cv-button-secondary" href="https://scixplorer.org/search?q=author%3A%22van+Donkelaar%2C+Floor%22&sort=date+desc%2C+bibcode+desc&p_=0&d=astrophysics" target="_blank" rel="noopener noreferrer">Publications (SciX) &rarr;</a>
  </div>

  <section class="cv-feature" aria-labelledby="cv-appointment-heading">
    <span class="cv-eyebrow">Current appointment</span>
    <h2 id="cv-appointment-heading">Herchel Smith Postdoctoral Research Fellow</h2>
    <p><strong>University of Cambridge, United Kingdom</strong></p>
    <p>Institute of Astronomy &amp; Kavli Institute for Cosmology</p>
    <p class="cv-date">October 2025 &ndash; Present</p>
  </section>

  <section class="cv-section" aria-labelledby="cv-education-heading">
    <h2 class="cv-section-title" id="cv-education-heading">Education</h2>
    <div class="cv-education">

      <article class="cv-entry">
        <h3>PhD in Computational Astrophysics</h3>
        <p class="cv-institution">University of Zurich, Switzerland</p>
        <p class="cv-date">September 2021 &ndash; September 2025</p>
        <details><summary>Thesis &amp; details</summary><div class="cv-meta">
          <p><strong>Thesis:</strong>  <a href="https://lup.lub.lu.se/student-papers/search/publication/9047007" target="_blank" rel="noopener noreferrer"> Disc Galaxies and Their Components at High Redshift: Similarities with the Local Universe </a> </p>
          <p><strong>Supervisor:</strong> Prof. Dr. Lucio Mayer</p>
        </div></details>
      </article>

      <article class="cv-entry">
        <h3>MSc in Astrophysics</h3>
        <p class="cv-institution">Lund University, Sweden</p>
        <p class="cv-date">August 2019 &ndash; May 2021</p>
        <details><summary>Thesis &amp; details</summary><div class="cv-meta">
          <p><strong>Thesis:</strong> <a href="https://www.zora.uzh.ch/handle/20.500.14742/239463" target="_blank" rel="noopener noreferrer">The fate of stars born in gas-rich high redshift galaxies</a> </p>
          <p><strong>Supervisor:</strong> Prof. Dr. Oscar Agertz</p>
          <p><strong>GPA:</strong> 3.83 / 4.00</p>
          <p><strong>Distinguishing Coursework: </strong>  Extragalactic Astronomy, Computational Astrophysics, Statistical Tools in Astrophysics Modern &amp; Experimental Particle Physics </p>
        </div></details>
      </article>

      <article class="cv-entry">
        <h3>BSc in Sociotechnical Engineering</h3>
        <p class="cv-institution">University of Twente (ATLAS), The Netherlands</p>
        <p class="cv-date">September 2016 &ndash; July 2019</p>
        <details><summary>Thesis &amp; details</summary><div class="cv-meta">
          <p><strong>Thesis:</strong> The Star Formation Rate, Metallicity and Thermal Pressure in Galaxies at z = 0.4 using MUSE</p>
          <p><strong>Supervisor:</strong> Dr. Kasper Borello Schmidt (Leibniz-Institut f&uuml;r Astrophysik Potsdam)</p>
          <p><strong>GPA:</strong> 3.85 / 4.00</p>
          <p><strong>Minor:</strong> Physics and Astronomy (Lund University)</p> 
        </div></details>
      </article>

    </div>
  </section>

  <section class="cv-section" aria-labelledby="cv-supervision-heading">
    <h2 class="cv-section-title" id="cv-supervision-heading">Supervision &amp; Mentoring</h2>
    <p class="cv-institution">I enjoy working with students on research projects in galaxy formation and computational astrophysics.</p>
    <div class="cv-research-grid">
      <article class="cv-entry">
        <span class="cv-eyebrow">Master's students · Co-supervisor</span>
        <h3>Daniel Swinger</h3>
        <p class="cv-institution">ETH Zurich · 2025&ndash;2026</p>
        <p>Birth of galactic discs in the PHOEBOS simulation.</p>
        <!-- When published, replace the status below with: <a href="PAPER_URL">Read paper &rarr;</a> -->
        <p class="cv-paper-status">Paper in preparation</p>
        <h3>Xiaojie Liao</h3>
        <p class="cv-institution">University of Lancashire · 2026</p>
        <p>Bar properties in a high-redshift galaxy simulation.</p>
        <!-- When published, replace the status below with: <a href="PAPER_URL">Read paper &rarr;</a> -->
        <p class="cv-paper-status">Paper in preparation</p>
      </article>
      <article class="cv-entry">
        <span class="cv-eyebrow">Bachelor's student · Primary supervisor</span>
        <h3>Romy Jager</h3>
        <p class="cv-institution">University of Twente · 2026</p>
        <p>Disc stability and the Toomre parameter in GigaEris.</p>
      </article>
    </div>
  </section>

  <section class="cv-section" aria-labelledby="cv-award-heading">
    <h2 class="cv-section-title" id="cv-award-heading">Selected Award</h2>
    <article class="cv-entry">
      <h3><a href="https://ssaa.ch/en/edith_a_m_ller_award" target="_blank" rel="noopener noreferrer">Edith Alice Müller Award &rarr;</a></h3>
      <p class="cv-institution">Swiss Society for Astrophysics and Astronomy</p>
      <p class="cv-date">2026</p>
      <p>For an outstanding PhD thesis.</p>
    </article>
  </section>

  <section class="cv-section" aria-labelledby="cv-research-heading">
    <h2 class="cv-section-title" id="cv-research-heading">Early Research Experience</h2>
    <div class="cv-research-grid">

      <article class="cv-entry">
        <h3>Oxford University</h3>
        <p class="cv-role">Research Internship</p>
        <p class="cv-date">June 2020 &ndash; November 2020</p>
        <p>Analyzing GMCs in the Large Magellanic Cloud using N-body hydrodynamical simulations.</p>
        <p><strong>Supervisor:</strong> Dr. Kearn Grisdale</p>
      </article>

      <article class="cv-entry">
        <h3>Leibniz-Institut f&uuml;r Astrophysik, Potsdam</h3>
        <p class="cv-role">Summer Project</p>
        <p class="cv-date">July 2017</p>
        <p>Generating template spectra of MUSE-Wide emission line sources.</p>
        <p><strong>Supervisor:</strong> Dr. Kasper Borello Schmidt</p>
      </article>

    </div>
  </section>

</div>
