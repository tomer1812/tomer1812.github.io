---
layout: research
seo_title: "Hybrid Models for Intervention Outcomes | Tomer Meir"
title: "Hybrid models for intervention outcomes"
permalink: /projects-hybrid/
author_profile: true
excerpt: "Combining mechanistic knowledge and neural networks for robust prediction under time-dependent interventions."
---

**How can we predict how a patient will respond to a treatment we have not seen before?** A model can fit its training data well yet make unreliable predictions for a different patient population or treatment schedule. This matters when the goal is to compare possible interventions, rather than simply predict what usually happens.

## A motivating example: anesthesia

Consider selecting a propofol dose to reach a target drug concentration in the brain. The response depends on patient characteristics and how the drug moves through the body. Physiological models offer useful guidance, but their simplifying assumptions can miss important differences between patients. Neural networks can learn those differences, yet struggle outside the situations represented in their training data.

## Combining physiology with learning

We developed a **physical AI approach: a structured hybrid mechanistic model** that preserves a physiological model and learns corrections from data. It separates the effect of an intervention from the system's other dynamics. When physical parameters are unknown, an initial simulation-based training step helps infer them before learning the corrections.

## What we accomplished

We tested the approach on pendulum dynamics and a **semi-synthetic propofol dosing task** using characteristics from 12,155 MIMIC-IV patients, with simulated treatments and drug concentrations. The hybrid model selected doses more accurately than the mechanistic and fully data-driven baselines for held-out older and higher-BMI groups. The fully data-driven model performed best within the training distribution.

The result shows how scientific knowledge can support more robust predictions for unfamiliar patients and interventions. These experiments use schedules fixed in advance and demonstrate a research method, rather than clinically validated dosing performance.

## Paper

**Structured Hybrid Mechanistic Models for Robust Estimation of Time-Dependent Intervention Outcomes**\
Tomer Meir, Ori Linial, Danny Eytan, Uri Shalit\
*Preprint, 2026*

[Read the paper](https://arxiv.org/abs/2602.11350)
