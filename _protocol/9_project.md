---
layout: page
title: RFMIP2.0 Protocol
permalink: /protocol/
description: Details of the RFMIP2.0 Protocol
img: assets/img/6.jpg
importance: 4
category: fun
---

**UNDER CONSTRUCTION**

# RFMIP Experimental Protocol

The Radiative Forcing Model Intercomparison Project (RFMIP) defines standard simulations to quantify effective radiative forcing (ERF) and its components across climate models.

---

## Inferring Effective Radiative Forcing from Global Model Integrations

The primary goal of RFMIP2.0 is to characterize the Effective Radiative Forcing (ERF) across models and understand inter-model differences. The Effective Radiative Forcing includes rapid adjustments in the troposphere such as changes in clouds and vertical temperature structure, in addition to the well-known stratospheric adjustment that occurs in response to an abrupt change in greenhouse gas forcing. Rapid adjustments are distinct from climate feedbacks, which scale with changing near-surface air temperature. Rapid adjustments, including those driven by cloud changes, can be determined using radiative kernels and other diagnostic techniques.

The RFMIP2.0 protocol, like its predecessor, includes a suite of fixed sea-surface temperature 30-year time-slice experiments to robustly diagnose the ERF for a given perturbation and a suite of fixed sea-surface temperature transient simulations extending from 1850–2100, used to diagnose the time evolution of the ERF. The ERF will be diagnosed as the difference in net top-of-atmosphere radiative flux between each experiment and the model’s pre-industrial control run. Fixing sea-surface temperatures and sea-ice conditions suppresses climate feedbacks and allows ERF to be diagnosed as the difference in top-of-atmosphere (TOA) radiation fluxes between each experiment and the `piClim-control` run [(Forster et al., 2016)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2016JD025320). Experiments are ranked into Tiers to emphasize their priority level.

---

## 1. RFMIP2.0 Experiments

As noted, three legacy RFMIP experiments are now part of the CMIP7 DECK. While no longer technically RFMIP experiments, they are crucial for the project so we consider them Tier 1 RFMIP experiments here. Also as noted, some RFMIP experiments are part of the CMIP7 Assessment Fast Track (AFT).

The table below summarizes the fixed-SST time-slice experiments used to diagnose effective radiative forcing.

### Table 1: Fixed-SST 30yr Time-Slice Simulations

| Tier | Experiment ID | Description / Forcing | SST / Sea Ice Condition | Minimum Length |
| :---: | :--- | :--- | :--- | :---: |
| **DECK/Tier 1** | `piClim-control` | Baseline pre-industrial atmospheric state | Climatological 1850 SSTs | 30 Years |
| **DECK/Tier 1** | `piClim-4xCO2` | Abrupt $4 \times \text{CO}_2$ concentration increase | Climatological 1850 SSTs | 30 Years |
| **DECK/Tier 1** | `piClim-anthro` | All present-day (2021) anthropogenic forcings combined | Climatological 1850 SSTs | 30 Years |
| **AFT/Tier 1** | `piClim-aer` | Anthropogenic aerosols at present-day (2021) levels | Climatological 1850 SSTs | 30 Years |
| **Tier 1** | `piClim-ghg` | Well-mixed greenhouse gases at present-day (2021) levels | Climatological 1850 SSTs | 30 Years |
| **Tier 1** | `piClim-lu` | Present-day (2021) land use / land cover changes | Climatological 1850 SSTs | 30 Years |

---

### Table 2: Historical (1850–2021) / scen7-mc Medium Concentration Scenario (2022–2100) Fixed-SST Transient Simulations

| Tier | Experiment Title | Experiment Description | Start | End | Major Purposes |
| :--- | :--- | :--- | :---: | :---: | :--- |
| **AFT/Tier 1** | `piClim-histall` | Time-varying forcing from all agents | 1850 | 2100 | Diagnose transient ERF from all agents |
| **AFT/Tier 1** | `piClim-histaer` | Time-varying ERF from aerosols (ozone fixed at pre-industrial concentrations) | 1850 | 2100 | Diagnose transient ERF from aerosols (ozone fixed at pre-industrial) |
| **AFT/Tier 2** | `piClim-histnat` | Time-varying ERF from volcanoes, solar (including spectral) variability, etc. | 1850 | 2100 | Diagnose transient natural ERF |
| **AFT/Tier 2** | `piClim-histghg` | Time-varying ERF from non-ozone (well-mixed) greenhouse gases | 1850 | 2100 | Diagnose transient ERF from non-ozone greenhouse gases |

---

> **UNDER CONSTRUCTION:** More to come. See full protocol in [Kramer et al., 2026](https://gmd.copernicus.org/articles/19/4447/2026/).
