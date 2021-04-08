---
layout: pub
title:  "Automated Detection of Many-Particle Solvation States for Accurate Characterizations of Diffusion Kinetics"
journal: "J. Chem. Phys."
authors: "J. F. Rudzinski, M. Radu & T. Bereau"
details: "MMMK, 024102"
year: "2019"
jlink: "https://aip.scitation.org/doi/10.1063/1.5064808"
preprint: "https://arxiv.org/pdf/1810.03528.pdf"
data: "https://github.com/JFRudzinski/Scripts_for_Automated_detection_of_many-particle_solvation_states"
data-label: "Scripts/Data"
data-title: "Scripts and examples for hidden-Markov-model-based configuration-space discretization"
pub-id: "JCP_Rudzinski_Bereau_2019"
date:   2019-01-08 00:00:00 +0100
categories: jekyll Pub
pubtitlepic: Fig
pubtitlepic_suff: jpg
abstract: 'Discrete-space kinetic models, i.e., Markov state models, have emerged as powerful tools for reducing the complexity of trajectories generated from molecular dynamics simulations. These models require configuration-space representations that accurately characterize the relevant dynamics. Well-established, low-dimensional order parameters for constructing this representation have led to widespread application of Markov state models to study conformational dynamics in biomolecular systems. On the contrary, applications to characterize single-molecule diffusion processes have been scarce and typically employ system-specific, higher-dimensional order parameters to characterize the local solvation state of the molecule. In this work, we propose an automated method for generating a coarse configuration-space representation, using generic features of the solvation structure—the coordination numbers about each particle. To overcome the inherent noisy behavior of these low-dimensional observables, we treat the features as indicators of an underlying, latent Markov process. The resulting hidden Markov models filter the trajectories of each feature into the most likely latent solvation state at each time step. The filtered trajectories are then used to construct a configuration-space discretization, which accurately describes the diffusion kinetics. The method is validated on a standard model for glassy liquids, where particle jumps between local cages determine the diffusion properties of the system. Not only do the resulting models provide quantitatively accurate characterizations of the diffusion constant, but they also reveal a mechanistic description of diffusive jumps, quantifying the heterogeneity of local diffusion.'
bullets:
  - "Special issue: <i>Markov Models of Molecular Kinetics</i>"
---