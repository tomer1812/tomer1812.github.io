---
layout: research
seo_title: "MISTR: Treatment Effects in Survival Data | Tomer Meir"
title: "Personalized treatment effects with censored outcomes"
permalink: /projects-hte-tte/
author_profile: true
excerpt: "MISTR: estimating heterogeneous treatment effects when survival outcomes are incompletely observed."
---

**Which patients benefit most from a treatment, and by how much?** For survival outcomes, that question is difficult because follow-up often ends before the event occurs. These right-censored observations contain useful information that treatment-effect models need to account for.

We developed **MISTR (Multiple Imputation for Survival Treatment Response)**. It uses recursively imputed survival trees to create plausible completed datasets, estimates treatment effects in each, and combines the results. This avoids directly estimating the censoring distribution and makes existing treatment-effect learners usable with censored outcomes.

## Evidence and contribution

- Improved estimation under heavy censoring in simulations and semi-synthetic experiments based on MIMIC-IV patient data.
- An application to the ACTG 175 HIV trial, estimating how treatment benefits vary with patient characteristics.
- An extension for unobserved confounding when a valid instrumental variable is available, evaluated on an unemployment-benefit dataset.

<img src="figure1.png" alt="MISTR workflow: multiply impute censored survival outcomes, estimate treatment effects, and combine estimates" width="600">

*Multiple imputation makes incomplete survival outcomes usable for heterogeneous treatment-effect estimation.*

## Paper and code

**Heterogeneous Treatment Effect in Time-to-Event Outcomes: Harnessing Censored Data with Recursively Imputed Trees**\
Tomer Meir, Uri Shalit, Malka Gorfine\
*ICML, 2025*

[Paper](https://arxiv.org/abs/2502.01575) · [ICML](https://icml.cc/virtual/2025/poster/45413) · [Code](https://github.com/tomer1812/mistr)
