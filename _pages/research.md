---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---
{% include base_path %}

<style>
  /* Research page: same palette and panels as Outreach & Media and Academic CV. */
  .research-page {
    --research-accent: #97a2cf;
    --research-link: #586a9e;
    --research-text: #414654;
    --research-muted: #667085;
    --research-tint: #f5f6fc;
    --research-border: #e7e9f2;
    color: var(--research-text);
    container: research-page / inline-size;
  }

  .research-page * { box-sizing: border-box; }
  .research-page a { color: var(--research-link); }
  .research-page a:hover { text-decoration: underline; }
  .research-page a:focus-visible {
    outline: 3px solid var(--research-accent);
    outline-offset: 3px;
  }
  .research-page p { margin-top: 0; line-height: 1.55; }
  .research-page .research-intro {
    margin: .15rem 0 1rem;
    font-size: .94rem;
  }

  /* The image is the feature. Keep all four panels and scale labels visible. */
  .research-page .research-feature {
    margin: .25rem 0 2.05rem;
    padding: .55rem;
    overflow: hidden;
    border: 1px solid var(--research-border);
    border-top: 4px solid var(--research-accent);
    border-radius: 12px;
    background: var(--research-tint);
  }
  .research-page .research-feature img {
    display: block;
    width: 100%;
    height: auto;
    border-radius: 7px;
    background: #10101b;
  }
  .research-page .research-feature figcaption {
    padding: .8rem .55rem .35rem;
    color: var(--research-muted);
    font-size: .79rem;
    line-height: 1.5;
  }
  .research-page .research-feature figcaption strong {
    color: var(--research-text);
  }

  /* Three research themes, laid out like the Outreach cards. */
  .research-page .research-section { margin: 0 0 1.9rem; }
  .research-page .research-section h2 {
    margin: 0 0 .45rem;
    font-size: 1.4rem;
    line-height: 1.3;
  }
  .research-page .research-section-intro {
    margin-bottom: 1rem;
    color: var(--research-muted);
    font-size: .9rem;
  }
  .research-page .research-grid {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: .95rem;
  }
  .research-page .research-card {
    display: flex;
    flex-direction: column;
    min-width: 0;
    padding: 1.05rem 1rem 1.1rem;
    border: 1px solid var(--research-border);
    border-top: 3px solid var(--research-accent);
    border-radius: 10px;
    background: #fff;
  }
  .research-page .research-eyebrow {
    display: block;
    margin: 0 0 .5rem;
    color: var(--research-link);
    font-size: .68rem;
    font-weight: 750;
    letter-spacing: .055em;
    text-transform: uppercase;
  }
  .research-page .research-card h3 {
    margin: 0 0 .6rem;
    font-size: 1.07rem;
    line-height: 1.33;
  }
  .research-page .research-card p {
    margin-bottom: .65rem;
    font-size: .85rem;
  }
  .research-page .research-card p:last-child { margin-bottom: 0; }
  .research-page .research-card-link {
    margin-top: auto;
    padding-top: .35rem;
    font-weight: 650;
  }

  .research-page .research-more {
    margin: 0 0 1rem;
    padding: .9rem 1.1rem;
    border-left: 4px solid var(--research-accent);
    border-radius: 0 9px 9px 0;
    background: var(--research-tint);
    font-size: .89rem;
  }
  .research-page .research-more p { margin: 0; }

  /* AcademicPages' sidebar leaves a narrower article than the browser window. */
  @container research-page (min-width: 680px) {
    .research-page .research-grid { grid-template-columns: repeat(3, minmax(0, 1fr)); }
  }
  @container research-page (max-width: 430px) {
    .research-page .research-feature { padding: .3rem; }
    .research-page .research-feature figcaption { padding: .7rem .45rem .4rem; }
    .research-page .research-card { padding: .95rem; }
  }
</style>

<div class="research-page">

  <p class="research-intro">
    How do the first galaxies build their discs and star clusters? I use cosmological simulations to study how these structures form, evolve and shape the galaxies we see today.
  </p>

  <figure class="research-feature">
    <img
      src="{{ '/images/massiveblack.png' | relative_url }}"
      alt="MassiveBlackPS simulation: an early galaxy in its cosmic environment, a zoom into its galactic disc, and close-up views of gas and stars in a compact cluster."
      loading="eager">
    <figcaption>
      <strong>From galaxies to star clusters.</strong> A multi-scale view of the <em>MassiveBlackPS</em> simulation, from the surrounding gas to the compact gas and stellar structures within an early galaxy.
    </figcaption>
  </figure>

  <section class="research-section" aria-labelledby="research-themes-heading">
    <h2 id="research-themes-heading">What I work on</h2>
    <p class="research-section-intro">Discs, clusters and the gas connecting them.</p>

    <div class="research-grid">
      <article class="research-card">
        <span class="research-eyebrow">GigaEris &amp; PHOEBOS</span>
        <h3>The first galactic discs</h3>
        <p>
          Some galaxies already have rotating discs when the Universe is very young. With <em>PHOEBOS</em>, I study when these discs first appear and what sets them apart from other galaxies. With <em>GigaEris</em>, I follow what happens to early discs as their galaxies grow.
        </p>
        <p class="research-card-link">
          <a href="https://ui.adsabs.harvard.edu/abs/2025MNRAS.539.1259V/abstract" target="_blank" rel="noopener noreferrer">Read about GigaEris &rarr;</a>
        </p>
      </article>

      <article class="research-card">
        <span class="research-eyebrow">MassiveBlackPS</span>
        <h3>Star clusters &amp; cosmic wallflowers</h3>
        <p>
          Early galaxies form remarkably compact star clusters, both within their discs and in the gas surrounding them. I study how these different birth environments affect cluster rotation and evolution, including possible links to globular clusters, nuclear star clusters and intermediate-mass black holes.
        </p>
        <p class="research-card-link">
          <a href="https://arxiv.org/abs/2601.05333" target="_blank" rel="noopener noreferrer">Meet the cosmic wallflowers &rarr;</a>
        </p>
      </article>

      <article class="research-card">
        <span class="research-eyebrow">FABLE &amp; FABLE-SE</span>
        <h3>Feedback &amp; circumgalactic clumps</h3>
        <p>
          What happens to dense gas outside galaxies? With <em>FABLE</em> and <em>FABLE-SE</em>, I investigate how feedback affects clump formation, migration and survival in the circumgalactic medium. I also test how simulation resolution changes what we identify as a clump.
        </p>
        <p class="research-card-link">Ongoing research</p>
      </article>
    </div>
  </section>

  <div class="research-more">
    <p>Interested in the details? You can find my papers and preprints on the <a href="{{ '/publications/' | relative_url }}">publications page &rarr;</a></p>
  </div>

</div>
