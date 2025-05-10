---
title: "Learning the essential in less than 2k additional weights- a simple approach to improve image classification stability
under corruptions"
teaser: "/images/2024_06_Learning_the_Essential_in_less_than_2k_additional_weights-a_single_large_kernel_convolution_layer_can_improve_prediction_stability_under_unknown_corruptions_Kernel_Architecture.pdf"
collection: publications
permalink: /publication/2024_06_Learning_the_Essential_in_less_than_2k_additional_weights
excerpt: ''
date: 2024-06-10
venue: 'Transactions on Machine Learning Research'
paperurl: ''
citation: 'K. Baeuerle, P. Mueller, S. M. Kazim, I. Ihrke, and M. Keuper, &quot;Learning the essential in less than 2k additional weights- a simple approach to improve image classification stability,&quot; <i>Transactions on Machine Learning Research</i>, Jun. 2024'
---
Abstract -- The performance of image classification on well-known benchmarks such as ImageNet is remarkable, but in safety-critical situations, the accuracy often drops significantly under adverse conditions. To counteract these performance drops, we propose a very simple modification to the models: we pre-pend a single, dimension preserving convolutional layer with a large linear kernel whose purpose it is to extract the information that is essential for image classification. We show that our simple modification can increase the robustness against common corruptions significantly, especially for corruptions of high severity. We demonstrate the impact of our channel-specific layers on ImageNet-100 and ImageNette classification tasks and show an increase of up to 30% accuracy on corrupted data in the top1 accuracy. Further, we conduct a set of designed experiments to qualify the conditions for our findings. Our main result is that a data- and network-dependent linear subspace carries the most important classification information (the essential), which our proposed pre-processing layer approximately identifies for most corruptions, and at very low cost.

[Download paper here](2024_06_Learning_the_Essential_in_less_than_2k_additional_weights-a_single_large_kernel_convolution_layer_can_improve_prediction_stability_under_unknown_corruptions.pdf)
