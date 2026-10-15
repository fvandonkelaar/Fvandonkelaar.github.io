---
layout: archive
title: "Outreach & Media"
permalink: /outreach/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

<style>
  /* Scoped to this page so it does not affect the rest of the website. */
  .outreach-page {
    --outreach-accent: #97a2cf;
    --outreach-link: #586a9e;
    --outreach-text: #414654;
    --outreach-muted: #667085;
    --outreach-tint: #f5f6fc;
    --outreach-border: #e7e9f2;
    max-width: 100%;
    color: var(--outreach-text);
  }

  .outreach-page * { box-sizing: border-box; }
  .outreach-page a { color: var(--outreach-link); }
  .outreach-page a:hover { text-decoration: underline; }
  .outreach-page a:focus-visible { outline: 3px solid var(--outreach-accent); outline-offset: 3px; }
  .outreach-page p { margin-top: 0; line-height: 1.65; }

  .outreach-intro {
    max-width: 48rem;
    margin: 0 0 2.1rem;
    font-size: 1.02rem;
    line-height: 1.75;
  }

  .outreach-eyebrow {
    display: block;
    margin: 0 0 .55rem;
    color: var(--outreach-link);
    font-size: .70rem;
    font-weight: 750;
    letter-spacing: .11em;
    text-transform: uppercase;
  }

  /* The main BBC feature */
  .outreach-feature {
    margin: 0 0 2.8rem;
    padding: clamp(1.1rem, 3vw, 2rem);
    border: 1px solid var(--outreach-border);
    border-top: 4px solid var(--outreach-accent);
    border-radius: 12px;
    background: var(--outreach-tint);
  }

  .outreach-feature h2 {
    margin: 0 0 1.35rem;
    font-size: clamp(1.42rem, 2.9vw, 1.9rem);
    line-height: 1.25;
    font-weight: 700;
  }

  .outreach-feature-grid {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: 1.4rem;
    align-items: center;
  }

  .outreach-feature-copy p { margin-bottom: 1rem; }
  .outreach-feature-copy p:last-of-type { margin-bottom: 1.2rem; }

  .outreach-actions {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: .75rem 1.1rem;
  }

  .outreach-page .outreach-button {
    display: inline-block;
    padding: .76rem 1rem;
    border: 1px solid #6b79aa;
    border-radius: 6px;
    background: #6b79aa;
    color: #fff;
    font-weight: 650;
    font-size: .82rem;
    line-height: 1.35;
    text-decoration: none;
    text-align: center;
    transition: background .15s ease, border-color .15s ease;
  }

  .outreach-page .outreach-button:hover {
    background: #526291;
    border-color: #526291;
    color: #fff;
    text-decoration: none;
  }

  .outreach-page .outreach-text-link {
    font-size: .85rem;
    font-weight: 650;
    text-decoration: none;
  }

  .outreach-embed {
    width: 100%;
    min-width: 0;
    padding: .7rem;
    background: #fff;
    border: 1px solid var(--outreach-border);
    border-radius: 9px;
    text-align: center;
  }

  .outreach-embed .twitter-tweet { margin: .3rem auto !important; }
  .outreach-embed-note {
    margin: .65rem 0 .2rem !important;
    font-size: .71rem;
    color: var(--outreach-muted);
    line-height: 1.45 !important;
  }

  /* More recent outreach work */
  .outreach-section { margin: 0 0 2.7rem; }
  .outreach-section h2 {
    margin: 0 0 .6rem;
    font-size: 1.4rem;
    line-height: 1.3;
  }
  .outreach-section-intro {
    margin-bottom: 1.3rem !important;
    color: var(--outreach-muted);
    font-size: .9rem;
  }

  .outreach-card-grid {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: 1.1rem;
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
    height: 145px;
    object-fit: cover;
    object-position: center;
  }

  .outreach-iwd-art {
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(135deg, #edeefa 0%, #dce0f5 100%);
    color: #526291;
    text-align: center;
    font-size: 1.28rem;
    line-height: 1.25;
    font-weight: 750;
    letter-spacing: .01em;
  }
  .outreach-iwd-art span { display: block; }
  .outreach-iwd-art small { display: block; margin-top: .4rem; font-size: .68rem; letter-spacing: .09em; text-transform: uppercase; }
  .outreach-card-content { padding: 1.15rem 1.2rem 1.2rem; }
  .outreach-card h3 {
    margin: 0 0 .55rem;
    font-size: 1.04rem;
    line-height: 1.3;
  }
  .outreach-card p { margin-bottom: .8rem; font-size: .83rem; }
  .outreach-card p:last-child { margin-bottom: 0; }
  .outreach-card-links { font-weight: 600; }

  /* Earlier activities are present, but visually quieter. */
  .outreach-past .outreach-card {
    background: #fbfbfd;
    border-color: #ececf2;
  }
  .outreach-past .outreach-card-image { height: 115px; }
  .outreach-past .outreach-card-content { padding: 1rem 1.15rem; }

  .outreach-contact {
    margin: .5rem 0 1rem;
    padding: 1.45rem 1.55rem;
    border-left: 4px solid var(--outreach-accent);
    background: var(--outreach-tint);
    border-radius: 0 9px 9px 0;
  }
  .outreach-contact h2 { margin: 0 0 .5rem; font-size: 1.25rem; }
  .outreach-contact p { margin-bottom: .9rem; font-size: .9rem; }

  @media (min-width: 690px) {
    .outreach-feature-grid { grid-template-columns: minmax(0, .92fr) minmax(0, 1.08fr); }
    .outreach-card-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  }

  @media (max-width: 430px) {
    .outreach-feature { padding: 1rem; }
    .outreach-page .outreach-button { width: 100%; }
    .outreach-actions { align-items: stretch; }
    .outreach-embed { padding: .35rem; }
  }
</style>

<div class="outreach-page">

  <p class="outreach-intro">
    I spend a lot of my time thinking about how the first galaxies formed, but I also really enjoy sharing that science beyond academia. Whether it's through television, public talks or community projects, I like making astronomy a little more accessible (and hopefully getting a few more people excited about it!).
  </p>

  <section class="outreach-feature" aria-labelledby="outreach-bbc-heading">
    <span class="outreach-eyebrow">Featured on BBC Four · October 2026</span>
    <h2 id="outreach-bbc-heading">Clumpy galaxies, dyslexia &amp; <em>The Sky at Night</em></h2>

    <div class="outreach-feature-grid">
      <div class="outreach-feature-copy">
        <p>
          In October 2026, I joined Maggie Aderin-Pocock on the BBC's <em>The Sky at Night</em> for an episode called <em>Space for Different Perspectives</em>.
        </p>
        <p>
          We talked about why the earliest galaxies are so clumpy, how I use simulations to study them, and how being dyslexic has shaped the way I approach science. Seeing my galaxies on television was a pretty surreal experience!
        </p>
        <div class="outreach-actions">
          <a class="outreach-button" href="https://www.bbc.co.uk/programmes/m0032wv0" target="_blank" rel="noopener noreferrer">Watch the BBC episode &rarr;</a>
          <a class="outreach-text-link" href="https://x.com/BBCStargazing/status/2110687128791183636" target="_blank" rel="noopener noreferrer">Watch the short clip &rarr;</a>
        </div>
      </div>

      <div class="outreach-embed" aria-label="BBC Stargazing video post">
        <!-- X converts this blockquote into the embedded post and its video.
             The link remains useful if a visitor blocks social media embeds. -->
        <blockquote class="twitter-tweet" data-dnt="true" data-theme="light" data-align="center">
          <a href="https://x.com/BBCStargazing/status/2110687128791183636">Watch my BBC Stargazing clip on X</a>
        </blockquote>
        <p class="outreach-embed-note">
          Video not showing? <a href="https://x.com/BBCStargazing/status/2110687128791183636" target="_blank" rel="noopener noreferrer">Open the clip on X</a>.
        </p>
      </div>
    </div>
  </section>

  <section class="outreach-section" aria-labelledby="outreach-science-heading">
    <h2 id="outreach-science-heading">Sharing science</h2>
    <p class="outreach-section-intro">A few other ways I've been involved in science communication and outreach.</p>

    <div class="outreach-card-grid">
      <article class="outreach-card">
        <img class="outreach-card-image" src="https://github.com/user-attachments/assets/dff52865-d5f4-4b6f-9bd8-f6a43f38c401" alt="Astronomy outreach" loading="lazy">
        <div class="outreach-card-content">
          <h3>Talks &amp; podcasts</h3>
          <p>
            I enjoy sharing my research and the slightly winding route that brought me into astronomy. I've given talks at alumni events for the University of Twente, and my work on wandering black holes was also discussed on <em>The StarXiv</em> podcast.
          </p>
          <p class="outreach-card-links">
            <a href="https://www.utwente.nl/en/alumni/events/2023/9/1097040/twente4tu-alumni-event-zurich-27th-september-2023" target="_blank" rel="noopener noreferrer">Alumni talk &rarr;</a>
            &nbsp;·&nbsp;
            <a href="https://starxiv.com/2025/05/12/episode-11-whirling-planes-wandering-black-holes-and-alien-supernovae/" target="_blank" rel="noopener noreferrer">StarXiv podcast &rarr;</a>
          </p>
        </div>
      </article>

      <article class="outreach-card">
        <div class="outreach-card-image outreach-iwd-art" role="img" aria-label="International Women's Day 2026 at Cambridge">
          <span>International Women's Day<small>Cambridge · 2026</small></span>
        </div>
        <div class="outreach-card-content">
          <h3>Women in astronomy</h3>
          <p>
            In 2026, I co-chaired the International Women's Day initiative at the Institute of Astronomy in Cambridge. Together, we organised events to celebrate women in astronomy, while also highlighting the challenges that still exist in our field.
          </p>
        </div>
      </article>
    </div>
  </section>

  <section class="outreach-section outreach-past" aria-labelledby="outreach-earlier-heading">
    <h2 id="outreach-earlier-heading">Earlier projects &amp; community involvement</h2>
    <p class="outreach-section-intro">Not all of my outreach has been about astronomy!</p>

    <div class="outreach-card-grid">
      <article class="outreach-card">
        <img class="outreach-card-image" src="https://github.com/user-attachments/assets/a9b3d2cb-e352-4536-ad34-899fb0ed97ca" alt="Lund University alumni community" loading="lazy">
        <div class="outreach-card-content">
          <h3>Alumni community</h3>
          <p>
            I was a Lund University Alumni Ambassador, helping incoming students make the most of their time at Lund. From 2021 to 2022, I also served as Chair and PR Manager of the <a href="https://www.uct-alumni.nl/" target="_blank" rel="noopener noreferrer">UCT Alumni Association</a>, where I worked on alumni connections and introduced projects such as <a href="https://www.linkedin.com/pulse/alumni-abroad-z%C3%BCrich-uct-alumni/" target="_blank" rel="noopener noreferrer">alumni blogs</a>.
          </p>
        </div>
      </article>

      <article class="outreach-card">
        <img class="outreach-card-image" src="https://github.com/user-attachments/assets/45af1ddb-14e8-4a5f-b4bd-d178f3ec8402" alt="Rugby community and social media" loading="lazy">
        <div class="outreach-card-content">
          <h3>Rugby community</h3>
          <p>
            Another passion of mine is rugby. I previously worked as a PR manager and graphic designer for rugby teams, helping double our social media following and increase engagement by 40%. I'm not as involved in that side of rugby anymore, but I'm still rather proud of what we achieved!
          </p>
        </div>
      </article>
    </div>
  </section>

  <section class="outreach-contact" aria-labelledby="outreach-contact-heading">
    <h2 id="outreach-contact-heading">Let's talk astronomy!</h2>
    <p>
      Looking for someone to give a talk, join a podcast or chat about science? I'd love to hear from you.
    </p>
    <a class="outreach-button" href="mailto:fv294@cam.ac.uk">Get in touch &rarr;</a>
  </section>

</div>

<!-- Load once, after the embedded post. -->
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
