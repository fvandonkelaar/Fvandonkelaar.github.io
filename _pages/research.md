---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

My research focuses on the formation and evolution of galaxies, with a specific emphasis on the structural assembly of Milky Way-sized systems. By utilizing state-of-the-art cosmological hydrodynamical simulations, I aim to bridge the gap between high-redshift observations, such as those from the James Webb Space Telescope (JWST) and ALMA, and the detailed galactic archeology of our own local Universe.

## Early Galaxy Formation
Recent observations reveal that the first galaxies were surprisingly massive, luminous, and structurally mature even at redshifts greater than nine. Morphological studies indicate that many of these early galaxies already exhibited disc-like structures by redshift four. These findings suggest that galaxy formation and structural assembly occurred earlier and more efficiently than previously predicted.

Cosmological hydrodynamical simulations provide a framework to interpret these results. The PHOEBOS simulation adopts intentionally weak stellar feedback and no AGN feedback. At redshifts above eight, it reproduces key galaxy properties such as the stellar mass function, the stellar-to-halo mass relation, specific star formation rates, and the size-to-mass slope. Weak feedback allows galaxies to remain bright and grow massive without over-suppressing star formation, providing a natural explanation for the abundance of bright, disc-dominated galaxies in the early Universe. To match observations at lower redshift, feedback must evolve. Stronger stellar or AGN feedback slows star formation and galaxy growth after redshift six. Weak stellar feedback at high redshift explains the early bright, structured galaxies, while evolving feedback is necessary to reproduce later cosmic trends.

## The Fate of Primordial Discs
One of the major pillars of my research is exploring the longevity and evolution of the first (kinematically cold) stellar discs. Using the high-resolution GigaEris simulation, I investigate how these primordial structures survive or transform through the chaotic environments of the early universe (z > 4). Understanding whether these early discs persist to form the modern "thin disc" of galaxies like the Milky Way is critical for a complete theory of galactic morphology.

Work done in PHOEBOS complements this work by showing that at z>8, a small fraction of galaxies host rotationally supported discs. These discs occur almost exclusively in the highest-mass haloes. They exhibit lower gas temperatures, younger stellar populations, and larger halo sizes and masses compared to non-disc systems. Understanding whether these early discs persist to form the modern thin discs of galaxies like the Milky Way is crucial for a complete theory of galactic morphology.

## Star Clusters
Another major pillar are the dense stellar environments found at the hearts of galaxies, but also within the filaments. My work explores:
- **Proto-Globular Clusters**: Studying the birth and migration of early star clusters in the circum-galactic medium.
- **High-Redshift Dense Clusters**: Investigating how galactic disc fragmentation and gravitational collapse along filaments at redshifts above seven can form ultracompact clusters. These dense clusters can also seed intermediate-mass black holes, which may later grow into supermassive black holes. Observations show that many early galaxies host extremely dense, compact stellar clusters at redshifts above six, and our simulations reproduce this behavior both within discs and along filaments.
- **Feedback in Dense Clusters**: Dense stellar clusters modify the local impact of feedback. Clustered supernovae inject more momentum than isolated events, scaling superlinearly with cluster size. Concentrated radiation, winds, and ionization fields boost local heating and gas pressure. Feedback is more efficient locally, while large-scale effects may be limited if energy is trapped. These processes must be captured to fully understand early galaxy growth.
- **Origin of the Nuclear Star Cluster**: identifying a hybrid formation scenario for the Milky Way's NSC. Using high-resolution simulations, I have shown that the NSC is built both from the dynamical in-spiral of primordial globular clusters and local in-situ star formation fueled by gas channeled to the center by early stellar bars. This process is intrinsically linked to the formation of the Nuclear Stellar Ring (NSR) at z > 4.

## Intermediate-Mass Black Holes (IMBHs)
The "missing link" of black hole evolution, the IMBHs, is a recurring theme in my simulations. I assess the reality of wandering IMBHs within Milky Way-mass galaxies, determining whether these elusive objects are likely to be found in the stellar halos of modern galaxies or if they remain hidden within massive clusters. You could say they are a bit mide side quest. 

## Computational Methods
I utilize and develop numerical tools, including smoothed-particle hydrodynamics (SPH) with metal-line cooling and thermal diffusion, to model the multi-phase interstellar medium. My work relies on massive "zoom-in" simulations that allow for the resolution of individual star clusters within a larger cosmological context. Most of my work is done using Changa, but I'm slowly transitioning into also using Arepo.
