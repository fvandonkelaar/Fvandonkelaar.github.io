---
permalink: /
title: "About"
excerpt: "Floor van Donkelaar"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
{% include base_path %}

<style>
  .about-page {
    --about-accent: #97a2cf;
    --about-link: #586a9e;
    --about-text: #414654;
    --about-muted: #667085;
    --about-tint: #f5f6fc;
    --about-border: #e7e9f2;
    color: var(--about-text);
  }
  .about-page * { box-sizing: border-box; }
  .about-page p { margin-top: 0; line-height: 1.6; font-size: .94rem; }
  .about-page a { color: var(--about-link); }
  .about-page .about-hello { margin: .1rem 0 1.2rem; font-size: 1rem; }
  .about-page .about-feature {
    margin: 0 0 1.1rem;
    padding: 1.25rem 1.35rem;
    border: 1px solid var(--about-border);
    border-top: 4px solid var(--about-accent);
    border-radius: 12px;
    background: var(--about-tint);
  }
  .about-page .about-feature h2, .about-page .about-card h2 {
    margin: 0 0 .65rem; font-size: 1.24rem;
  }
  .about-page .about-feature p:last-child, .about-page .about-card p:last-child { margin-bottom: 0; }
  .about-page .about-grid { display: grid; grid-template-columns: 1fr; gap: 1rem; margin-bottom: 1.4rem; }
  .about-page .about-card {
    padding: 1.1rem 1.2rem;
    border: 1px solid var(--about-border);
    border-top: 3px solid var(--about-accent);
    border-radius: 10px;
    background: #fff;
  }
  .about-page .about-links { margin-top: .85rem; font-size: .86rem; font-weight: 650; }
  .about-page .about-small { color: var(--about-muted); font-size: .9rem; }
  @media (min-width: 900px) {
    .about-page .about-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  }
</style>

<div class="about-page">

  <p style="font-size: 0.75rem; color: #8a90a3; margin-bottom: 1.5rem;">
  Last updated: 16 October 2026
</p>

  <p class="about-hello"><strong>Hej, everyone!</strong> I'm Floor van Donkelaar, a computational astrophysicist and Herchel Smith Postdoctoral Research Fellow at the Institute of Astronomy and Kavli Institute for Cosmology at the University of Cambridge.</p>

  <section class="about-feature">
    <h2>What I study</h2>
   <p>
  I use cosmological simulations to study the <strong>formation and evolution
  of dense stellar systems</strong>, particularly star clusters and clumps,
  in the early Universe. I am especially interested in where these
  structures form, how their environments shape their evolution,
  and what they might become. Alongside this, I study the formation
  of the first galactic discs.
</p>
    <p class="about-links"><a href="/research/">More about my research &rarr;</a> &nbsp;·&nbsp; <a href="https://scixplorer.org/search?q=author%3A%22van+Donkelaar%2C+Floor%22&sort=date+desc%2C+bibcode+desc&p_=0&d=astrophysics">My publications &rarr;</a></p>
  </section>

  <div class="about-grid">
    <section class="about-card">
      <h2>My journey</h2>
      <p>I completed my PhD at the University of Zürich with Lucio Mayer, after studying astrophysics at Lund University and sociotechnical engineering at the University of Twente. And now you can find me in Cambridge :).</p>
      <p class="about-links" style="margin-top: auto;"><a href="/cv/">Academic CV &rarr;</a></p>
    </section>
    <section class="about-card">
      <h2>Beyond research</h2>
      <p>Outside work, you'll often find me on a rugby pitch, cycling or exploring somewhere new. I also enjoy sharing science and bringing people together. Recently, I even got to talk about galaxies and dyslexia on the BBC's <em>The Sky at Night</em>!</p>
      <p class="about-links" style="margin-top: auto;"><a href="/outreach/">Outreach &rarr;</a>  &nbsp;·&nbsp; <a href="https://cambridgerugby.co.uk/women/">Rugby &rarr;</a>  &nbsp;·&nbsp; <a href="https://www.strava.com/athletes/62259659">Strava &rarr;</a> </p>
    </section>
  </div>
</div>
