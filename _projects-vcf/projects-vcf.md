---
layout: research
seo_title: "Deep Learning for Vertebral Fracture Detection | Tomer Meir"
title: "Detecting vertebral fractures in CT"
permalink: /projects-vcf/
author_profile: true
excerpt: "A compact spine representation and 3D sequence model for vertebral compression fracture detection."
---

**Routine CT scans can reveal vertebral compression fractures that otherwise go undiagnosed.** Identifying them can help flag patients who may benefit from osteoporosis assessment and treatment.

At **Zebra Medical Vision**, I helped develop an automated system that locates the spinal cord, builds a compact representation of the spine, and analyzes sequences of 3D vertebral patches. The approach reduces the memory demands of processing full CT volumes while retaining information relevant to fracture detection.

## Results

The study compared representations and model architectures, including a 3D convolutional sequence-to-sequence network. An ensemble achieved a **patient-level AUC of 0.955** on the study's evaluation dataset.

<img src="vcf-algo.png" alt="Fracture-detection pipeline from CT scan through spine localization, compact representation, and 3D sequence classification" width="1000">

*From a full CT scan to a compact spine representation and fracture prediction.*

## Paper

**3D Convolutional Sequence to Sequence Model for Vertebral Compression Fractures Identification in CT**\
David Chettrit\*, Tomer Meir\*, Hila Lebel, Mila Orlovsky, Ronen Gordon, Ayelet Akselrod-Ballin, Amir Bar\
*MICCAI, 2020* · *\*Equal contribution.*

[Read the paper](https://arxiv.org/abs/2010.03739)
