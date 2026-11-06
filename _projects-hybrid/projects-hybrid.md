---
layout: research
seo_title: "Hybrid Models for Intervention Outcomes | Tomer Meir"
title: "Hybrid models for intervention outcomes"
permalink: /projects-hybrid/
author_profile: true
excerpt: "Combining mechanistic knowledge and neural networks for robust prediction under time-dependent interventions."
---

**How can we predict a patient's response to an intervention beyond the data we trained on?** Mechanistic models encode physiology but can miss important dynamics. Neural networks learn flexible relationships but can struggle with unfamiliar patients or treatment schedules.

We developed a structured hybrid model that combines a mechanistic core with learned corrections, explicitly separating intervention-dependent dynamics from the rest of the system. When mechanistic parameters are unknown, an encoder is first trained on simulations; the mechanistic component is then held fixed while correction networks learn from observed trajectories.

## Evidence

We evaluated the approach on pendulum dynamics and a **semi-synthetic propofol dosing task** using characteristics from 12,155 MIMIC-IV patients, with simulated treatments and drug-concentration trajectories. The hybrid model achieved lower dose-selection error than the mechanistic and fully data-driven baselines in held-out older and higher-BMI groups. The fully data-driven model performed best within the training distribution.

The work demonstrates how scientific structure can improve generalization when predicting intervention outcomes. The experiments consider treatment schedules fixed in advance and do not establish clinical dosing performance.

## Paper

**Structured Hybrid Mechanistic Models for Robust Estimation of Time-Dependent Intervention Outcomes**\
Tomer Meir, Ori Linial, Danny Eytan, Uri Shalit\
*Preprint, 2026*

[Read the paper](https://arxiv.org/abs/2602.11350)
