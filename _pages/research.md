---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

My big goal would be to uncover some of the missing steps in the process of galaxy formation, especially at high redshift and the influence of star clusters (one can dream, right?). Telescopes have already revealed their present-day beauty and now with e.g. JWST we now also get a look on how they looked at higher redshift, but the path from these basic "blops" to fully-formed galaxies remains a puzzle. Imagine it as if we're putting together a complex piece of furniture, using an IKEA manual. We've got the list of parts (stars, gas, and dark matter) and we know what the finished product should look like (galaxies). What we're after are the instructions that bridge the gap, those vital steps in between. I have been working on bridging this gap in understanding galaxy formation by using powerfull simulations, I mainly focus on the formation and evolution of galactic structures in Milky Way analogues. 

## The Simulations
To understand how high-redshift galactic structures evolve into the galactic features we see today, I have been using high-resolution zoom-in simulations such as GigaEris and Phoebos.  These advanced N-body and hydrodynamical simulations will allow us to investigate how early cosmic structures develop into key components like gaseous discs and stellar bulges. **GigaEris** is like a detailed microscope, zooming in on the formation of a Milky Way-sized galaxy halo. The simulation employs a modern implementation of smoothed-particle hydrodynamics, including metal-line cooling and metal and thermal diffusion. This simulation helps us focus on how galaxies assemble in their early stages, going down to redshift z = 4.4. 

![bigplot_page-0001 (2)](https://github.com/fvandonkelaar/Fvandonkelaar.github.io/assets/57528256/c0938e10-5dd7-4b3d-9c4d-c2bbabd4eb3a)

These high-resolution zoom-in simulations will need to be complemented by large-scale simulations to capture the broader environment, especially the influence of massive galaxy clusters and their interactions at these high redshifts, one such simulation that can be used is the **Phoebos**. This simulation will act as a broader view, covering a larger uniform volume of the cosmos. It's like a wide-angle lens, examining the cosmic web and structure formation in a significant volume from an earlier redshift of z = 249.  

Combining these simulations help us with gaining insight into the formation of galaxies, illustrating the transition from fundamental elements such as stars and gas to more complex baryonic structures, including the formation of the nuclear star cluster and/or the formation of stellar discs at high redshift galaxies.

## The Evolution of the Galactic Structures 
During my PhD, I have tried to shed light on the unique structures and dynamics that should distinguish high-redshift galaxies from their modern counterparts. By  analyzing the properties of various stellar clusters, including Globular and Nuclear Star Clusters, as well as the galactic disc, we have found that key features such as disc formation and stellar clustering were already present in early galaxies, mirroring those in local galaxies today. In a recent study <a href="https://ui.adsabs.harvard.edu/abs/2024arXiv240611960V/abstract">(van Donkelaar et al., 2024b)</a>, we identified a critical link between the (pseudo-)bulge and the kinematically cold disc, proposing a groundbreaking "two-phase" disc formation process, in which the early disc evolves into the pseudo-bulge at high redshifts. Earlier work revealed that stars from this kinematically thin disc eventually contribute to the formation of the Nuclear Star Cluster <a href="https://ui.adsabs.harvard.edu/abs/2023arXiv230312828V/abstract">(van Donkelaar et al., 2024a)</a>, offering a new hybrid model for cluster formation. While this does not capture the full complexity of high-redshift galaxies, reframing our understanding of these early systems will provide deeper insights into the processes of galaxy formation and evolution.

![image](https://github.com/user-attachments/assets/ea0efa6c-4e1d-4dfe-9ecd-dd4d3a2b45a2)

Additionally, I have integrated my experience with GigaEris and simulations run with the grid-based code RAMSES to study the neutral gas fraction of a galaxy and its impact on disc formation (e.g., [van Donkelaar et al., 2022](https://ui.adsabs.harvard.edu/abs/2022MNRAS.512.3806V/abstract); Agertz et al., in prep.).


### Star Cluster Formation 
In my research on the evolution of galactic structures, I have primarily focused on the formation of star clusters and their impact on galactic morphology. In my first PhD paper  <a href="https://ui.adsabs.harvard.edu/abs/2023MNRAS.522.1726V/abstract">(van Donkelaar et al., 2023)</a>, we found that nearly all proto-globular clusters (proto indicating the presence of dark matter in their halos, with a minimum baryon fraction of 75%) in our study formed within gas filaments directed towards the galaxy. Additionally, every proto-GC was located within 5 kpc of a dark matter subhalo, consistent with the formation mechanism proposed by <a href="https://ui.adsabs.harvard.edu/abs/2020ApJ...890...18M/abstract">(Madau et al., 2020)</a>. Notably, the stellar masses of the proto-GCs in our study were comparable to those described by Madau et al.

![Presentation1](https://github.com/user-attachments/assets/1e3ff8f7-d5a5-48e1-9585-35bc5da27186)

However, star clusters can also form within the galaxy itself. In <a href="https://ui.adsabs.harvard.edu/abs/2023arXiv230312828V/abstract"> van Donkelaar et al. (2024a)</a>, we demonstrated that baryon-dominated clusters formed in the galaxy's center, specifically in a nuclear ring. This is expected in a barred galaxy system, where the bar efficiently funnels gas toward the center, a phenomenon that is also evident in my findings. There are, of course, other mechanisms through which star clusters form, such as Toomre instabilities in the disc. However, to better understand the influence of these formations, it is essential to incorporate a star cluster *subgrid model* into the simulation. This approach will allow for more accurate modeling of star cluster formation and evolution in high-redshift environments, a task I am currently working on.

