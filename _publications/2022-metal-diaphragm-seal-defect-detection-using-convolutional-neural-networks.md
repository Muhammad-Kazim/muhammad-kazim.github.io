---
title: "Metal Diaphragm Seal Defect Detection Using Convolutional Neural Networks"
collection: publications
permalink: /publication/2022-02-metal-diaphragm-seal-defect-detection-using-convolutional-neural-networks
excerpt: ''
date: 2022-02-02
venue: ''
paperurl: ''
citation: 'S. M. Kazim, J. Tayyub, M. Sarmad, and Patrick Werner, &quot;Metal Diaphragm Seal Defect Detection Using Convolutional Neural Networks,&quot; Feb. 2022'
---
Abstract -- Vision-based defect detection of manufactured parts is a process that largely requires manual inspection and verification. This is a laborious task which uses precious worker time as well as being repetitive and mundane. We tackle the problem of fine-grained defect detection on shiny and reflective metal diaphragm seals. We propose to use a convolutional neural network (CNN) that can detect defects on images of metal surfaces with concentric rings texture. Our proposed pipeline consists of a localization and a detection stage. The localization module isolates a circular region of interest (ROI) in an image by using a CNN-based circle detector. A detection module then predicts a segmentation map of the ROI by segmenting out each detected defect. Defected parts are then identified by aggregating defected segments and thresholding total defected area to a certain value. This value is chosen by domain experts. The developed system is deployed in a real industrial setting and continuous worker feedback is used for evaluation. We demonstrate the superiority of our approach through extensive experimentation and ablations studies.

[Download paper here](http://muhammad-kazim.github.io/files/2022-metal-diaphragm-seal-defect-detection-using-convolutional-neural-networks.pdf)