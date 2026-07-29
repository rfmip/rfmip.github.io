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

The Radiative Forcing Model Intercomparison Project (RFMIP) defines standard simulations to quantify Effective Radiative Forcing (ERF) and its components across climate models.

---

## Inferring Effective Radiative Forcing from Global Model Integrations

The RFMIP2.0 protocol, like its predecessor, includes a suite of fixed sea-surface temperature 30-year *time-slice experiments* to robustly diagnose the ERF for a given perturbation and a suite of fixed sea-surface temperature *transient experiments* extending from 1850–2100, used to diagnose the time evolution of the ERF. Fixing sea-surface temperatures and sea-ice conditions suppresses climate feedbacks and allows ERF to be diagnosed as the difference in top-of-atmosphere (TOA) radiation fluxes between each experiment and the `piClim-control` run [(Forster et al., 2016)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2016JD025320). Experiments are ranked into Tiers to emphasize their priority level.

---

## 1. Tier 1 and Tier 2 Core RFMIP2.0 Experiments

As noted in the tables below, three legacy RFMIP experiments are now part of the CMIP7 DECK. While no longer technically RFMIP experiments, they are crucial for the project and we consider them Tier 1 RFMIP experiments here. Also as noted, some RFMIP experiments are part of the CMIP7 Assessment Fast Track (AFT).

&nbsp;
&nbsp;

### Table 1: Fixed-SST 30yr Time-Slice Simulations

| Tier | Experiment ID | Description / Forcing | SST / Sea Ice Condition | Minimum Length |
| :---: | :--- | :--- | :--- | :---: |
| Tier 1/DECK | `piClim-control` | Baseline pre-industrial atmospheric state | Climatological 1850 SSTs | 30 Years |
| Tier 1/DECK | `piClim-4xCO2` | Abrupt $4 \times \text{CO}_2$ concentration increase | Climatological 1850 SSTs | 30 Years |
| Tier 1/DECK | `piClim-anthro` | All present-day (2021) anthropogenic forcings combined | Climatological 1850 SSTs | 30 Years |
| Tier 1/AFT | `piClim-aer` | Anthropogenic aerosols at present-day (2021) levels | Climatological 1850 SSTs | 30 Years |
| Tier 1 | `piClim-ghg` | Well-mixed greenhouse gases at present-day (2021) levels | Climatological 1850 SSTs | 30 Years |
| Tier 1 | `piClim-lu` | Present-day (2021) land use / land cover changes | Climatological 1850 SSTs | 30 Years |

---

&nbsp;
&nbsp;

### Table 2: Fixed-SST Transient Simulations - Historical (1850–2021) / scen7-mc Medium Concentration Scenario (2022–2100) 

| Tier | Experiment Title | Experiment Description | Start | End | Major Purposes |
| :--- | :--- | :--- | :---: | :---: | :--- |
| Tier 1/AFT | `piClim-histall` | Time-varying forcing from all agents | 1850 | 2100 | Diagnose transient ERF from all agents |
| Tier 1/AFT | `piClim-histaer` | Time-varying ERF from aerosols (ozone fixed at pre-industrial concentrations) | 1850 | 2100 | Diagnose transient ERF from aerosols (ozone fixed at pre-industrial) |
| Tier 2/AFT | `piClim-histnat` | Time-varying ERF from volcanoes, solar (including spectral) variability, etc. | 1850 | 2100 | Diagnose transient natural ERF |
| Tier 2/AFT | `piClim-histghg` | Time-varying ERF from non-ozone (well-mixed) greenhouse gases | 1850 | 2100 | Diagnose transient ERF from non-ozone greenhouse gases |

---

## 2. Tier 3 RFMIP2.0 Experiments

Tier 3 consists of new fixed-SST time-slice experiments to study the linearity of radiative forcing, the sensitivity of radiative forcing to the underlying base state, and the contribution of land effects on the diagnosis of radiative forcing.

## Table 3: Fixed-SST Time-Slice Experiments with +4K Warmert SSTs

| Tier | Experiment ID | Description / Forcing | SST / Sea Ice Condition | Minimum Length |
| :---: | :--- | :--- | :--- | :---: |
| Tier 3 | `piClim-p4K` | Pre-industrial (1850) conditions but with sea surface temperatures uniformly 4 K warmer | Uniformly 4 K warmer than pre-industrial | 30 Years |
| Tier 3  | `piClim-p4K-4xCO2` | CO2 concentrations set to 4 times pre-industrial with sea surface temperatures uniformly 4 K warmer than pre-industrial | Uniformly 4 K warmer than pre-industrial | 30 Years |
| Tier 3 | `piClim-p4K-aer` | Present day (2021) aerosols with sea surface temperatures uniformly 4 K warmer than pre-industrial | Uniformly 4 K warmer than pre-industrial | 30 Years |

--
&nbsp;
&nbsp;

## Table 4: Additional Perturbed Carbon Dioxide Fixed-SST Time-Slice Experiments

| Tier | Experiment ID | Description / Forcing | SST / Sea Ice Condition | Minimum Length |
| :---: | :--- | :--- | :--- | :---: |
| Tier 3 | `piClim-0.5xCO2` | CO2 concentrations set to half of pre-industrial | Climatological 1850 SSTs | 30 Years |
| Tier 3 | `piClim-2xCO2` | CO2 concentrations set to 2 times pre-industrial | Climatological 1850 SSTs | 30 Years |
| Tier 3 | `piClim-4xCO2-bgc` | CO2 concentrations set to 4 times pre-industrial applied only to carbon cycle | Climatological 1850 SSTs | 30 Years |
| Tier 3 | `piClim-4xCO2-rad` | CO2 concentrations set to 4 times pre-industrial applied only to radiation | Climatological 1850 SSTs | 30 Years |

--
&nbsp;
&nbsp;

## Table 5: Fixed-SST + Fixed-Land Surface Temperature Time-Slice Experiments

| Tier | Experiment ID | Description / Forcing | SST / Sea Ice Condition | Minimum Length |
| :---: | :--- | :--- | :--- | :---: |
| Tier 3 | `piClim-FixedLST` | Pre-industrial (1850) conditions with land-surface temperatures fixed from `piClim-control` | Climatological 1850 SSTs (Fixed LST) | 30 Years |
| Tier 3 | `piClim-FixedLST-4xCO2` | CO2 concentrations set to 4 times pre-industrial with land surface temperatures fixed at pre-industrial | Climatological 1850 SSTs (Fixed LST) | 30 Years |
| Tier 3 | `piClim-FixedLST-anthro` | Present-day (2021) anthropogenic forcing (greenhouse gases, aerosols, and land use) with land surface temperatures fixed at pre-industrial | Climatological 1850 SSTs (Fixed LST) | 30 Years |
| Tier 3 | `piClim-FixedLST-aer` | Present-day (2021) anthropogenic aerosols with land surface temperatures fixed at pre-industrial | Climatological 1850 SSTs (Fixed LST) | 30 Years |
| Tier 3 | `piClim-FixedLST-ghg` | Present-day (2021) well-mixed greenhouse gases only (non-ozone) with land surface temperatures fixed at pre-industrial | Climatological 1850 SSTs (Fixed LST) | 30 Years |
| Tier 3 | `piClim-FixedLST-lu` | Present-day (2021) land use with land surface temperatures fixed at pre-industrial | Climatological 1850 SSTs (Fixed LST) | 30 Years |

See full protocol details in [Kramer et al., 2026](https://gmd.copernicus.org/articles/19/4447/2026/) and
