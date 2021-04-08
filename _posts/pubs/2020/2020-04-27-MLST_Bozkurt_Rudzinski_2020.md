---
layout: pub
title:  "Interpretable Embeddings for Molecular Kinetics using Gaussian Mixture Variational Autoencoders"
journal: "Mach. Learn.: Sci. Technol."
authors: "Y. Bozkurt Varolgüneş, T. Bereau & J. F. Rudzinski"
details: "1, 015012"
year: "2020"
jlink: "https://iopscience.iop.org/article/10.1088/2632-2153/ab80b7"
preprint: "https://arxiv.org/pdf/1912.12175.pdf"
data: "https://github.com/yabozkurt/gmvae"
data-label: "Software"
data-title: "Gaussian mixture variational autoencoder implementation in TensorFlow"
pub-id: "MLST_Bozkurt_Rudzinski_2020"
date:   2020-04-27 00:00:00 +0100
categories: jekyll Pub
pubtitlepic: Fig
pubtitlepic_suff: jpg
abstract: 'Extracting insight from the enormous quantity of data generated from molecular simulations requires the identification of a small number of collective variables whose corresponding low-dimensional free-energy landscape retains the essential features of the underlying system. Data-driven techniques provide a systematic route to constructing this landscape, without the need for extensive a priori intuition into the relevant driving forces. In particular, autoencoders are powerful tools for dimensionality reduction, as they naturally force an information bottleneck and, thereby, a low-dimensional embedding of the essential features. While variational autoencoders ensure continuity of the embedding by assuming a unimodal Gaussian prior, this is at odds with the multi-basin free-energy landscapes that typically arise from the identification of meaningful collective variables. In this work, we incorporate this physical intuition into the prior by employing a Gaussian mixture variational autoencoder (GMVAE), which encourages the separation of metastable states within the embedding. The GMVAE performs dimensionality reduction and clustering within a single unified framework, and is capable of identifying the inherent dimensionality of the input data, in terms of the number of Gaussians required to categorize the data. We illustrate our approach on two toy models, alanine dipeptide, and a challenging disordered peptide ensemble, demonstrating the enhanced clustering effect of the GMVAE prior compared to standard VAEs. The resulting embeddings appear to be promising representations for constructing Markov state models, highlighting the transferability of the dimensionality reduction from static equilibrium properties to dynamics.'
#bullets:
#  - ""
---