---
layout: archive
title: "Vertebral Compression Fracture Identification from Computed Tomography"
permalink: /projects-vcf/
author_profile: true
---

An osteoporosis-related fracture occurs every three seconds worldwide, affecting one in three women and one in five men aged over 50. 
The early detection of at-risk patients facilitates effective and well evidenced preventative interventions, reducing the incidence of major osteoporotic fractures. 
In [this study](https://arxiv.org/abs/2010.03739) (Chettrit and Meir et al., 2020), presented in Medical Image Computing and Computer Assisted Intervention - 23rd - MICCAI (2020) conference, we present an automatic system for identification of vertebral compression fractures on Computed Tomography images.

First, we create a compact 3D representation of the spine using region of interest along the chest-abdomen CT scan by detecting the spinal cord region in the CT scan. 
Then, we use a novel end-to-end sequence to sequence 3D architecture (Fig. 1). 
We evaluate several model architectures and representations and present a framework combining an ensemble of models that achieves state of the art results, validated on a large data set. 

<img src="vcf-algo.png" alt="vcf" width="1000">
*Figure 1. Vertebral Compression Fractures Detection Algorithm.*


## Key Contributions
- The proposed system has been employed by healthcare providers to support clinical osteoporosis management. 
- Evaluation of different architectures and representations.