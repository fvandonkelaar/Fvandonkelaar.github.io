---
layout: archive
title: "Outreach & Media"
permalink: /outreach/
author_profile: true
---
{% include base_path %}

<style>
  /* All styles are scoped to the outreach page. */
  .outreach-page {
    --outreach-accent: #97a2cf;
    --outreach-link: #586a9e;
    --outreach-text: #414654;
    --outreach-muted: #667085;
    --outreach-tint: #f5f6fc;
    --outreach-border: #e7e9f2;
    color: var(--outreach-text);
    container: outreach / inline-size;
  }

  .outreach-page * { box-sizing: border-box; }
  .outreach-page a { color: var(--outreach-link); }
  .outreach-page a:hover { text-decoration: underline; }
  .outreach-page a:focus-visible { outline: 3px solid var(--outreach-accent); outline-offset: 3px; }
  .outreach-page p { margin-top: 0; line-height: 1.55; }
  .outreach-intro {
    margin: .15rem 0 1rem;
    font-size: .94rem;
  }

  /* Put the BBC video first, both visually and on smaller screens. */
  .outreach-feature {
    margin: .25rem 0 2.1rem;
    padding: clamp(.85rem, 2vw, 1.4rem);
    border: 1px solid var(--outreach-border);
    border-top: 4px solid var(--outreach-accent);
    border-radius: 12px;
    background: var(--outreach-tint);
  }
  .outreach-feature-grid {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: 1.1rem;
    align-items: start;
  }
  .outreach-embed {
    min-width: 0;
    padding: .4rem;
    border: 1px solid var(--outreach-border);
    border-radius: 9px;
    background: #fff;
    text-align: center;
  }
  .outreach-embed .twitter-tweet { margin: .2rem auto !important; }
  .outreach-embed-note {
    margin: .45rem .2rem .15rem !important;
    font-size: .74rem;
    color: var(--outreach-muted);
    line-height: 1.4 !important;
  }
  .outreach-feature-copy { padding-top: .1rem; }
  .outreach-eyebrow {
    display: block;
    margin: 0 0 .5rem;
    color: var(--outreach-link);
    font-size: .7rem;
    font-weight: 750;
    letter-spacing: .09em;
    text-transform: uppercase;
  }
  .outreach-feature h2 {
    margin: 0 0 .75rem;
    font-size: clamp(1.4rem, 2.6vw, 1.8rem);
    line-height: 1.26;
  }
  .outreach-feature-copy p {
    margin-bottom: .95rem;
    font-size: .91rem;
  }

  .outreach-page .outreach-button {
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
  .outreach-page .outreach-button:hover {
    background: #526291;
    border-color: #526291;
    color: #fff;
    text-decoration: none;
  }

  /* Three cards in one row on desktop, stacking on smaller screens. */
  .outreach-section { margin: 0 0 2.15rem; }
  .outreach-section h2 {
    margin: 0 0 .55rem;
    font-size: 1.4rem;
    line-height: 1.3;
  }
  .outreach-section-intro {
    margin-bottom: 1rem !important;
    color: var(--outreach-muted);
    font-size: .9rem;
  }
  .outreach-card-grid {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: .95rem;
  }
  .outreach-card {
    min-width: 0;
    overflow: hidden;
    border: 1px solid var(--outreach-border);
    border-radius: 10px;
    background: #fff;
  }
  .outreach-card-image {
    display: block;
    width: 100%;
    height: 270px;
    object-fit: contain;
    background: var(--outreach-tint);
    object-position: center;
  }
  .outreach-iwd-art {
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(135deg, #edeefa 0%, #dce0f5 100%);
    color: #526291;
    font-size: 1.08rem;
    font-weight: 750;
    line-height: 1.25;
    text-align: center;
  }
  .outreach-iwd-art small {
    display: block;
    margin-top: .4rem;
    font-size: .69rem;
    font-weight: 600;
    letter-spacing: .06em;
    text-transform: uppercase;
  }
  .outreach-card-content { padding: .95rem 1rem 1.1rem; }
  .outreach-card h3 { margin: 0 0 .5rem; font-size: 1.03rem; line-height: 1.3; }
  .outreach-card p { margin-bottom: .7rem; font-size: .85rem; }
  .outreach-card p:last-child { margin-bottom: 0; }
  .outreach-card-links { font-weight: 650; }

  .outreach-contact {
    margin: 0 0 1rem;
    padding: 1rem 1.2rem;
    border-left: 4px solid var(--outreach-accent);
    border-radius: 0 9px 9px 0;
    background: var(--outreach-tint);
  }
  .outreach-contact h2 { margin: 0 0 .35rem; font-size: 1.23rem; }
  .outreach-contact p { margin-bottom: .65rem; font-size: .9rem; }

  /* Respond to the article width, not the window width (AcademicPages has a sidebar). */
  @container outreach (min-width: 580px) {
    .outreach-feature-grid { grid-template-columns: minmax(0, 1.12fr) minmax(0, .88fr); }
  }
  @container outreach (min-width: 680px) {
    .outreach-card-grid { grid-template-columns: repeat(3, minmax(0, 1fr)); }
  }
  @container outreach (max-width: 430px) {
    .outreach-feature { padding: .7rem; }
    .outreach-embed { padding: .2rem; }
  }
</style>

<div class="outreach-page">

  <p class="outreach-intro">I enjoy sharing science beyond research papers, whether that's on TV, at public talks, or through community events.</p>

  <section class="outreach-feature" aria-labelledby="outreach-bbc-heading">
    <div class="outreach-feature-grid">
      <div class="outreach-embed" aria-label="BBC Stargazing video post">
        <!-- X replaces this with the actual video post when embeds are permitted. -->
        <blockquote class="twitter-tweet" data-dnt="true" data-theme="light" data-align="center">
          <a href="https://x.com/BBCStargazing/status/2110687128791183636">Watch my BBC Stargazing clip on X</a>
        </blockquote>
        <p class="outreach-embed-note">
          Video not showing? <a href="https://x.com/BBCStargazing/status/2110687128791183636" target="_blank" rel="noopener noreferrer">Watch the clip on X</a>.
        </p>
      </div>

      <div class="outreach-feature-copy">
        <span class="outreach-eyebrow">BBC Four · October 2026</span>
        <h2 id="outreach-bbc-heading">Clumpy galaxies, dyslexia &amp; <em>The Sky at Night</em></h2>
        <p>
          I joined Maggie Aderin-Pocock on the BBC's <em>The Sky at Night</em> to talk about the first clumpy galaxies, my simulations, and how being dyslexic shapes the way I approach science. Seeing my galaxies on TV was pretty surreal!
        </p>
        <a class="outreach-button" href="https://www.bbc.co.uk/programmes/m0032wv0" target="_blank" rel="noopener noreferrer">Watch the full episode &rarr;</a>
      </div>
    </div>
  </section>

  <section class="outreach-section" aria-labelledby="outreach-more-heading">
    <h2 id="outreach-more-heading">Beyond the BBC</h2>
    <p class="outreach-section-intro">From science talks to the communities and projects I care about.</p>

    <div class="outreach-card-grid">
      <article class="outreach-card">
        <img class="outreach-card-image" src="https://github.com/user-attachments/assets/dff52865-d5f4-4b6f-9bd8-f6a43f38c401" alt="Astronomy outreach" loading="lazy">
        <div class="outreach-card-content">
          <h3>Sharing science</h3>
          <p>
            I enjoy sharing my research and the route that brought me into astronomy. I've spoken at University of Twente alumni events, and my work was discussed on <em>The StarXiv</em> podcast.
          </p>
          <p class="outreach-card-links">
            <a href="https://www.utwente.nl/en/alumni/events/2023/9/1097040/twente4tu-alumni-event-zurich-27th-september-2023" target="_blank" rel="noopener noreferrer">Alumni talk &rarr;</a>
            &nbsp;·&nbsp;
            <a href="https://starxiv.com/2025/05/12/episode-11-whirling-planes-wandering-black-holes-and-alien-supernovae/" target="_blank" rel="noopener noreferrer">StarXiv &rarr;</a>
          </p>
        </div>
      </article>

      <article class="outreach-card">
        <div class="outreach-card-image outreach-iwd-art" role="img" aria-label="Science community at Cambridge">
          <span>Science community<small>Cambridge</small></span>
        </div>
        <div class="outreach-card-content">
          <h3>Supporting science</h3>
          <p>
            I enjoy helping make the astronomy community more welcoming and visible. At Cambridge, I have helped showcase research by early career scientists at the Institute of Astronomy and Kavli Institute, and co-chaired the 2026 International Women's Day initiative.
          </p>
        </div>
      </article>

      <article class="outreach-card">
        <img class="outreach-card-image" src="https://github.com/user-attachments/assets/3037fde6-918a-4295-87a2-d61876f9a5da" />
" alt="Green Team Twente celebrating with the trophy for the Shell Eco-marathon Communications Award" loading="lazy">
        <div class="outreach-card-content">
          <h3>Communication &amp; community</h3>
          <p>
            Long before astronomy, I enjoyed sharing stories and bringing people together. With Green Team Twente, our team won the 2018 Shell Eco-marathon Communications Award. I later served as Chair and PR Manager of the <a href="https://www.uct-alumni.nl/" target="_blank" rel="noopener noreferrer">UCT Alumni Association</a> (2021–2022), and as a Lund University Alumni Ambassador. I’ve also worked on PR for rugby teams.
          </p>
          <p class="outreach-card-links"><a href="https://www.utoday.nl/green-team-twente/65724/green-team-wins-communications-award" target="_blank" rel="noopener noreferrer">Green Team award &rarr;</a> &nbsp;·&nbsp; <a href="https://www.linkedin.com/pulse/alumni-abroad-z%C3%BCrich-uct-alumni/" target="_blank" rel="noopener noreferrer">Alumni blog &rarr;</a></p>
        </div>
      </article>
    </div>
  </section>

  <section class="outreach-contact" aria-labelledby="outreach-contact-heading">
    <h2 id="outreach-contact-heading">Let's talk astronomy!</h2>
    <p>Looking for someone to give a talk, join a podcast or chat about science? I'd love to hear from you.</p>
    <a class="outreach-button" href="mailto:fv294@cam.ac.uk">Get in touch &rarr;</a>
  </section>

</div>

<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
