---
title: "Deep Coded Wavefront Sensing: Bridging the Simulation-Experiment Gap"
teaser: "/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_2.png"
collection: publications
permalink: /publication/2025-09-Deep-Coded-Wavefront-Sensing-Bridging-the-Simulation-Experiment-Gap
excerpt: 'Selected for ***Oral*** presentation.'
date: 2025-09-23
venue: 'NeurIPS 2025 Workshop Learning to Sense (Proceedings Track)'
paperurl: 'https://openreview.net/pdf?id=4dQlpj6LHc'
citation: 'S. M. Kazim, P. Müller, and I. Ihrke, &quot;Deep Coded Wavefront Sensing: Bridging the Simulation-Experiment Gap,&quot; <i>NeurIPS 2025 Workshop Learning to Sense</i>, Sep. 2025'
---
Abstract -- Coded wavefront sensing (CWFS) is a recent computational quantitative phase imaging technique that enables one-shot phase retrieval of biological and other phase specimens. CWFS is readily integrable with standard laboratory microscopes and does not require specialized labor for its usage. The CWFS phase retrieval method is inspired by optical flow, but uses conventional optimization techniques. A main reason for this is the lack of publicly available datasets for CWFS, which prevents researchers from using deep neural networks in CWFS. In this paper, we present a forward model that utilizes wave optics to generate SynthBeads: a CWFS dataset obtained by modeling the complete experimental setup, including wave propagation through refractive index (RI) volumes of spherical microbeads, a standard microscope, and the phase mask, which is a key component of CWFS, with high fidelity. We show that our forward model enables deep CWFS, where pre-trained optical flow networks finetuned on SynthBeads successfully generalize to our SynthCell dataset, experimental microbead measurements, and, remarkably, complex biological specimens, providing quantitative phase estimates and thereby bridging the simulation-experiment gap.

## Principles of Coded Wavefront Sensing

## Forward Model Simulation

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_3.png" />
  <figcaption>Visualization 1: Abc.</figcaption>
</figure>

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_4.png" />
  <figcaption>Visualization 2: Abc.</figcaption>
</figure>

## SynthBeads and TestSynthCells: First-ever Datasets for Coded Wavefront Sensing

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_5.png" />
  <figcaption>Visualization 3: Abc.</figcaption>
</figure>

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_6.png" />
  <figcaption>Visualization 4: Abc.</figcaption>
</figure>

## Results on Synthetic and Real Data

