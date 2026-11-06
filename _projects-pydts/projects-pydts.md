---
layout: research
seo_title: "PyDTS: Survival Analysis with Competing Risks | Tomer Meir"
title: "Survival analysis with competing events and PyDTS"
permalink: /projects-pydts/
author_profile: true
excerpt: "Efficient discrete-time competing-risks regression and an open-source Python toolkit."
---

**When will a patient leave intensive care, and what will happen next?** Discharge home, transfer to another facility, and in-hospital death are competing events. When time is recorded in days, modeling these outcomes requires methods that account for both discrete time and competing risks.

We developed a **two-stage estimation procedure** for discrete-time competing-risks regression. Separating estimation of covariate effects from time-specific baseline parameters reduces computation and supports regularization and feature screening.

## Evidence and application

Simulation studies assessed estimation accuracy, confidence-interval coverage, and computation time. We applied the method to **25,170 MIMIC-IV ICU admissions**, modeling length of stay and the probabilities of discharge home, transfer, and in-hospital death over 28 days.

## PyDTS: from method to software

**PyDTS** provides the methods in an open-source Python package, with penalized regression, time-dependent covariates, feature screening, cross-validation, discrimination and calibration metrics, and synthetic-data generation.

[Documentation](https://tomer1812.github.io/pydts/) · [GitHub](https://github.com/tomer1812/pydts) · [PyPI](https://pypi.org/project/pydts/)

<img src="fitting_time_fig.png" alt="Simulation comparison of fitting times for the two-stage and data-expansion estimation procedures" width="600">

*Fitting-time comparison from the regression-methods study.*

## Papers

**Discrete-time Competing-Risks Regression with or without Penalization**\
Tomer Meir, Malka Gorfine\
*Biometrics, 2025* · [Paper](https://doi.org/10.1093/biomtc/ujaf040) · [Study code](https://github.com/tomer1812/DiscreteTimeSurvivalPenalization)

**PyDTS: A Python Package for Discrete-Time Survival Analysis with Competing Risks and Optional Penalization**\
Tomer Meir, Rom Gutman, Malka Gorfine\
*Journal of Open Source Software, 2025* · [Paper](https://doi.org/10.21105/joss.08815)
