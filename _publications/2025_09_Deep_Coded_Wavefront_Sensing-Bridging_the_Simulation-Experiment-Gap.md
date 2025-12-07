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

## Deep Coded Wavefront Sensing

Coded wavefront sensing (WFS) relates the gradient of the phase $ \nabla \phi $ at one plane (the phase mask) to the flow of pixels  in another (the image plane), a distance *z* away.

$$ I_1 (r) = I_0 (r + \frac{z}{k} \nabla\phi) $$.

<figure>
  <video width="800" height="400" loop autoplay muted controls>
    <source src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_10.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <figcaption>Visualization 1: <b>Principle of coded wavefront sensing.</b> The phase mask on top of the camera sensor creates speckles. These speckles move proportionally to the gradient of the wavefront compared to a reference speckle pattern.</figcaption>
</figure>

The purely optical flow relationship is only partially true in Coded WFS microscopy applications. The propagation of the wavefront by a distance *z* introduces amplitude variations as well as other features such as diffraction, which are inherent to microscopy. We propose leveraging pretrained optical flow networks by finetuning them with Coded WFS data, one that includes speckles, diffraction, and other microscopy features, so that the networks learn the mapping in the presence of these features, as shown below. 

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_9.png" />
  <figcaption>Visualization 2: <b>Deep coded wavefront sensing.</b> An optical flow network (RAFT here) is finetuned on synthetic Coded WFS data. A datapoint, which includes a tuple of reference and specimen speckle patterns and ground truth flow, is created by simulating wave optics effects as light traverses a volumetric object, through a microscope and a phase mask, and is finally incident on a camera sensor.</figcaption>
</figure>

## Forward Model Simulation

The entire coded WFS pipeline is accurately simulated using wave optical techniques. Our forward modeling maps the volumetric specimen in the object space to the image plane with high fidelity. The two major components include the microscope, mainly its NA (low pass filtering) and magnification, and the phase mask, which is responsible for the speckle pattern and the primary reason an ordinary camera is converted into an optical flow-based phase retrieval device.

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_3.png" />
  <figcaption>Visualization 3: <b> Schematic of our forward model</b>.</figcaption>
</figure>

We restrict our volumetric specimens to randomized configurations of spherical objects. By randomly sampling the number of spheres, their radii, positions, refractive indices, and phase mask features (height and smoothing), we ensure that the network does not overfit to specific distributions of objects and remains agnostic to phase mask distributions. Additionally, spheres can be simulated very accurately (and quickly) as shown below, and in the coded WFS setting, where the main features in image space are speckles, we believe the finetuned networks will generalize to non-spherical objects as well.

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_4.png" />
  <figcaption>Visualization 4: <b> Comaprison on simulated and experimentally measured focal stack of microspheres </b>.</figcaption>
</figure>

## SynthBeads and TestSynthCells: First-ever Datasets for Coded Wavefront Sensing

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_5.png" />
  <figcaption>Visualization 5: Abc.</figcaption>
</figure>

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_6.png" />
  <figcaption>Visualization 6: Abc.</figcaption>
</figure>

## Results on Synthetic and Real Data

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_7.png" />
  <figcaption>Visualization 7: Abc.</figcaption>
</figure>

<figure>
  <img width="400" height="400"
    src="/images/2025_09_Deep_Coded_Wavefront_Sensing_Bridging_the_Simulation-Experiment_Gap_8.png" />
  <figcaption>Visualization 8: Abc.</figcaption>
</figure>
