---
layout: research
seo_title: "Hybrid Models for Intervention Outcomes | Tomer Meir"
title: "Hybrid mechanistic–data-driven models for personalized time-dependent intervention outcomes"
permalink: /projects-hybrid/
author_profile: true
excerpt: "Combining mechanistic knowledge and neural networks for robust prediction under time-dependent interventions."
---

Patients respond differently to treatment. **How can we predict a patient's response to options they have not received, to help select the most suitable treatment?**

In medicine, treatments are often chosen based on patient characteristics. Comparing alternatives can therefore require predictions for patient–treatment combinations that are rare or absent in the observed data. This is an *out-of-distribution* challenge, where purely data-driven models can struggle.

We develop **hybrid mechanistic–data-driven models** that combine known physical dynamics with deep learning to make intervention-outcome predictions more robust under distribution shift.

## A motivating example: anesthesia

Consider selecting a propofol dose to reach a target drug concentration in the brain. The response depends on patient characteristics and how the drug moves through the body. Physiological models offer useful guidance but may miss important differences between patients. Neural networks can learn those differences, yet struggle beyond their training data.

For example, if older patients typically receive lower doses in the observed data, predicting their response to other doses is an out-of-distribution challenge where data-driven models struggle.

## Combining physiology with learning

We developed a **structured hybrid mechanistic–data-driven model** that keeps a mechanistic core and learns corrections from data. In the anesthesia example, this core is a pharmacokinetic model describing how the drug moves through the body. It separates intervention-related dynamics from the system's other dynamics. When physical parameters are unknown, an initial simulation-based training step helps infer effective model parameters before learning the corrections.

<figure class="hybrid-overview" aria-label="Conceptual overview of the hybrid model">
  <div class="hybrid-overview__flow">
    <div class="hybrid-overview__card"><strong>Scientific knowledge</strong><span>Known physical or physiological dynamics</span></div>
    <span class="hybrid-overview__operator" aria-hidden="true">+</span>
    <div class="hybrid-overview__card"><strong>Learned corrections</strong><span>Patterns learned from observed data</span></div>
    <span class="hybrid-overview__operator" aria-hidden="true">→</span>
    <div class="hybrid-overview__card hybrid-overview__result"><strong>Hybrid predictions</strong><span>Compare outcomes under different interventions</span></div>
  </div>
  <figcaption>Scientific knowledge anchors the model; learned corrections help account for what the mechanistic model misses.</figcaption>
</figure>

## What we accomplished

We tested the approach on pendulum dynamics and a semi-synthetic propofol dosing task using characteristics from 12,155 MIMIC-IV patients, with simulated treatments and drug concentrations. The hybrid model selected doses more accurately than the mechanistic and fully data-driven baselines for held-out older and higher-BMI groups.

**These results show how scientific knowledge can support more robust intervention-outcome predictions for unfamiliar patients and interventions.** The study evaluates predefined treatment schedules and simulated drug outcomes.

## Paper

**Structured Hybrid Mechanistic Models for Robust Estimation of Time-Dependent Intervention Outcomes**\
Tomer Meir, Ori Linial, Danny Eytan, Uri Shalit\
*Preprint, 2026*

[Read the paper](https://arxiv.org/abs/2602.11350)
