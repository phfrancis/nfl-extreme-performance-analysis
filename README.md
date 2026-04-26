# Extreme Performance Analysis of NFL Wide Receivers Using Simulation

This project uses simulation and extreme value modeling to analyze the fastest NFL wide receiver 40-yard dash performances and evaluate the reliability and stability of model estimates under varying sample sizes.

---

## Overview

This project investigates extreme athletic performance using NFL Combine wide receiver 40-yard dash data. The analysis focuses on the fastest performances and uses simulation to evaluate how extreme-value model estimates behave under different sample sizes.

The project applies a block-extremes framework, fits Generalized Extreme Value (GEV) models, computes return levels, and evaluates estimator performance using Monte Carlo simulation.

---

## Objectives

- Analyze annual fastest 40-yard dash performances among NFL wide receiver prospects  
- Model extreme performance using Generalized Extreme Value methods  
- Transform 40-yard dash times to a speed scale for interpretation  
- Evaluate bias, RMSE, and convergence behavior through simulation  
- Assess how estimator stability changes as record length increases  

---

## Methods

The analysis treats annual fastest 40-yard dash times as block extremes. Since smaller times indicate better performances, times are transformed to the negative-time scale so that faster performances correspond to larger values.

Monte Carlo simulations are used to generate annual block minima, fit GEV models, compute return levels, and evaluate the reliability and stability of model estimates across different sample sizes.

---

## Tools Used

- R  
- R Markdown  
- `dplyr`  
- `ggplot2`  
- `extRemes`  
- Monte Carlo simulation  
- Extreme Value Theory  

---

## Skills Demonstrated

- Statistical modeling (Extreme Value Theory, GEV)  
- Simulation and Monte Carlo methods  
- Data transformation and feature engineering  
- Model evaluation (bias, RMSE, convergence diagnostics)  
- Reproducible analysis using R Markdown  

---

## Key Outputs

- GEV model fitting for annual extreme performances  
- Return-level estimation on negative-time and speed scales  
- Bias and RMSE summaries  
- Convergence diagnostics across record lengths  
- Reproducible HTML report with figures and diagnostics  

---

## How to View Results

The full analysis and results are available in:

- `results/nfl_wr_gev_simulation.html`

Download and open this file in a web browser to view plots, diagnostics, and simulation outputs.

---

## Why This Matters

Extreme value modeling is widely used in risk analysis, finance, and engineering. This project demonstrates how simulation can be used to assess model reliability when working with limited data.

---

## Repository Structure

```bash
analysis/
    nfl_wr_gev_simulation.Rmd

results/
    nfl_wr_gev_simulation.html

appendix/
    Simulation-Based Verification.pdf
```
