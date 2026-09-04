---
layout: page
title: protocol
permalink: /protocol/
description: Details of the RFMIP2.0 Protocol.
nav: true
nav_order: 1
---

The Radiative Forcing Model Intercomparison Project defines standard simulations to quantify Effective Radiative Forcing (ERF) and its components across climate models.

## Inferring effective radiative forcing from global model integrations

The RFMIP2.0 protocol, like its predecessor, includes a suite of fixed sea-surface-temperature 30-year *time-slice experiments* to robustly diagnose the ERF for a given perturbation, and a suite of fixed sea-surface-temperature *transient experiments* extending from 1850–2100, used to diagnose the time evolution of the ERF. Fixing sea-surface temperatures and sea-ice conditions suppresses climate feedbacks and allows ERF to be diagnosed as the difference in top-of-atmosphere radiation fluxes between each experiment and the `piClim-control` run ([Forster et al., 2016](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2016JD025320)). Experiments are ranked into tiers to emphasize their priority level.

## 1. Tier 1 and Tier 2 core RFMIP2.0 experiments

Three legacy RFMIP experiments are now part of the CMIP7 DECK — while no longer technically RFMIP experiments, they remain crucial to the project and are treated as Tier 1 here. Some RFMIP experiments are also part of the CMIP7 Assessment Fast Track (AFT).

<div class="table-caption">Table 1 — <span>Fixed-SST 30-year time-slice simulations</span></div>
<div class="rfmip-table-wrap">
<table class="rfmip-table">
<tr><th>Tier</th><th>Experiment ID</th><th>Description / forcing</th><th>SST / sea ice condition</th><th>Min. length</th></tr>
<tr><td><span class="tier-badge tier-1">Tier 1 · DECK</span></td><td class="exp-id"><code>piClim-control</code></td><td class="desc">Baseline pre-industrial atmospheric state</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-1">Tier 1 · DECK</span></td><td class="exp-id"><code>piClim-4xCO2</code></td><td class="desc">Abrupt 4× CO₂ concentration increase</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-1">Tier 1 · DECK</span></td><td class="exp-id"><code>piClim-anthro</code></td><td class="desc">All present-day (2021) anthropogenic forcings combined</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-1">Tier 1 · AFT</span></td><td class="exp-id"><code>piClim-aer</code></td><td class="desc">Anthropogenic aerosols at present-day (2021) levels</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-1">Tier 1</span></td><td class="exp-id"><code>piClim-ghg</code></td><td class="desc">Well-mixed greenhouse gases at present-day (2021) levels</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-1">Tier 1</span></td><td class="exp-id"><code>piClim-lu</code></td><td class="desc">Present-day (2021) land use / land cover changes</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
</table>
</div>

<div class="table-caption">Table 2 — <span>Fixed-SST transient simulations, historical (1850–2021) / scen7-mc medium-concentration scenario (2022–2100)</span></div>
<div class="rfmip-table-wrap">
<table class="rfmip-table">
<tr><th>Tier</th><th>Experiment</th><th>Description</th><th>Start</th><th>End</th><th>Major purpose</th></tr>
<tr><td><span class="tier-badge tier-1">Tier 1 · AFT</span></td><td class="exp-id"><code>piClim-histall</code></td><td class="desc">Time-varying forcing from all agents</td><td>1850</td><td>2100</td><td>Diagnose transient ERF from all agents</td></tr>
<tr><td><span class="tier-badge tier-1">Tier 1 · AFT</span></td><td class="exp-id"><code>piClim-histaer</code></td><td class="desc">Time-varying ERF from aerosols (ozone fixed at pre-industrial concentrations)</td><td>1850</td><td>2100</td><td>Diagnose transient ERF from aerosols (ozone fixed at pre-industrial)</td></tr>
<tr><td><span class="tier-badge tier-2">Tier 2</span></td><td class="exp-id"><code>piClim-histnat</code></td><td class="desc">Time-varying ERF from volcanoes, solar (incl. spectral) variability, etc.</td><td>1850</td><td>2100</td><td>Diagnose transient natural ERF</td></tr>
<tr><td><span class="tier-badge tier-2">Tier 2</span></td><td class="exp-id"><code>piClim-histghg</code></td><td class="desc">Time-varying ERF from non-ozone (well-mixed) greenhouse gases</td><td>1850</td><td>2100</td><td>Diagnose transient ERF from non-ozone GHGs</td></tr>
</table>
</div>

## 2. Tier 3 RFMIP2.0 experiments

Tier 3 consists of new fixed-SST time-slice experiments to study the linearity of radiative forcing, the sensitivity of radiative forcing to the underlying base state, and the contribution of land effects to the diagnosis of radiative forcing.

<div class="table-caption">Table 3 — <span>Fixed-SST time-slice experiments with +4K warmer SSTs</span></div>
<div class="rfmip-table-wrap">
<table class="rfmip-table">
<tr><th>Tier</th><th>Experiment ID</th><th>Description / forcing</th><th>SST / sea ice condition</th><th>Min. length</th></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-p4K</code></td><td class="desc">Pre-industrial (1850) conditions with SSTs uniformly 4K warmer</td><td>Uniformly 4K warmer than pre-industrial</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-p4K-4xCO2</code></td><td class="desc">4× CO₂ with SSTs uniformly 4K warmer than pre-industrial</td><td>Uniformly 4K warmer than pre-industrial</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-p4K-aer</code></td><td class="desc">Present-day (2021) aerosols with SSTs uniformly 4K warmer than pre-industrial</td><td>Uniformly 4K warmer than pre-industrial</td><td>30 years</td></tr>
</table>
</div>

<div class="table-caption">Table 4 — <span>Additional perturbed CO₂ fixed-SST time-slice experiments</span></div>
<div class="rfmip-table-wrap">
<table class="rfmip-table">
<tr><th>Tier</th><th>Experiment ID</th><th>Description / forcing</th><th>SST / sea ice condition</th><th>Min. length</th></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-0.5xCO2</code></td><td class="desc">CO₂ concentrations set to half of pre-industrial</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-2xCO2</code></td><td class="desc">CO₂ concentrations set to 2× pre-industrial</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-4xCO2-bgc</code></td><td class="desc">CO₂ at 4× pre-industrial, applied only to the carbon cycle</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-4xCO2-rad</code></td><td class="desc">CO₂ at 4× pre-industrial, applied only to radiation</td><td>Climatological 1850 SSTs</td><td>30 years</td></tr>
</table>
</div>

<div class="table-caption">Table 5 — <span>Fixed-SST + fixed land-surface temperature time-slice experiments</span></div>
<div class="rfmip-table-wrap">
<table class="rfmip-table">
<tr><th>Tier</th><th>Experiment ID</th><th>Description / forcing</th><th>SST / sea ice condition</th><th>Min. length</th></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-FixedLST</code></td><td class="desc">Pre-industrial (1850) conditions with land-surface temperatures fixed from <code>piClim-control</code></td><td>Climatological 1850 SSTs (fixed LST)</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-FixedLST-4xCO2</code></td><td class="desc">4× CO₂ with land-surface temperatures fixed at pre-industrial</td><td>Climatological 1850 SSTs (fixed LST)</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-FixedLST-anthro</code></td><td class="desc">Present-day (2021) anthropogenic forcing (GHGs, aerosols, land use) with land-surface temperatures fixed at pre-industrial</td><td>Climatological 1850 SSTs (fixed LST)</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-FixedLST-aer</code></td><td class="desc">Present-day (2021) anthropogenic aerosols with land-surface temperatures fixed at pre-industrial</td><td>Climatological 1850 SSTs (fixed LST)</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-FixedLST-ghg</code></td><td class="desc">Present-day (2021) well-mixed greenhouse gases only (non-ozone) with land-surface temperatures fixed at pre-industrial</td><td>Climatological 1850 SSTs (fixed LST)</td><td>30 years</td></tr>
<tr><td><span class="tier-badge tier-3">Tier 3</span></td><td class="exp-id"><code>piClim-FixedLST-lu</code></td><td class="desc">Present-day (2021) land use with land-surface temperatures fixed at pre-industrial</td><td>Climatological 1850 SSTs (fixed LST)</td><td>30 years</td></tr>
</table>
</div>

## Lineage

RFMIP2.0 extends the original RFMIP protocol designed for CMIP6 by Pincus, Forster & Stevens (2016), carrying its fixed-SST approach forward with an updated design for the CMIP7 ensemble.

See full protocol details in [Kramer et al., 2026](https://gmd.copernicus.org/articles/19/4447/2026/).
