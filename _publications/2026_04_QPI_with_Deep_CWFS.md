---
title: "Quantitative phase imaging with deep coded wavefront sensing"
teaser: "/images/2026_04_Quantitative phase imaging with deep coded wavefront sensing.png"
collection: publications
permalink: /publication/2026_04_QPI_with_Deep_CWFS
date: 2026-04-16
excerpt: ""
venue: Optica Open
paperurl: 'https://preprints.opticaopen.org/articles/preprint/Quantitative_phase_imaging_with_deep_coded_wavefront_sensing/31902724'
citation: 'S. M. Kazim, P. Müller, A. Nehrych, and I. Ihrke, &quot; Quantitative phase imaging with deep coded wavefront sensing,&quot; <i>Optica Open</i>, Apr. 2026'
---
Abstract -- Coded wavefront sensing (CWFS) is an inexpensive, high-resolution quantitative phase imaging method that can be readily integrated into standard laboratory microscopes. However, conventional optical flow-based phase retrieval methods simplify the CWFS forward model by neglecting wave-optical effects such as diffraction to make the optimization tractable. This reduces the range of recoverable wavefront curvatures and limits the allowable phase mask-sensor distances. Our goal is to leverage the forward model without explicit calibration to enhance the QPI capabilities of CWFS. To this end, we introduce a wave-optical CWFS simulator that generates a synthetic dataset of 18,500 samples for supervised training of state-of-the-art optical flow neural networks, implicitly embedding the physics of the forward model into the network through data. We show that this Deep CWFS approach yields an 11 dB improvement in mean squared error on synthetic data and achieves a threefold expansion of the range of recoverable curvatures across practical mask-sensor distances. Despite being trained exclusively on simulated data, Deep CWFS generalizes seamlessly to several biological cell specimens, producing high-fidelity phase maps validated by digital holographic microscopy. Moreover, Deep CWFS is robust to variations in microscopes and phase masks because of the diversity of optical systems represented in the dataset.
