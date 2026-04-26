# Extreme Performance Analysis of NFL Wide Receivers Using Simulation

## Overview

This project investigates extreme athletic performance using NFL Combine wide receiver 40-yard dash data. The analysis focuses on the fastest performances and uses simulation to evaluate how extreme-value model estimates behave under different sample sizes.

The project applies a block-extremes framework, fits Generalized Extreme Value (GEV) models, computes return levels, and evaluates estimator performance using Monte Carlo simulation.

## Objectives

- Analyze annual fastest 40-yard dash performances among NFL wide receiver prospects
- Model extreme performance using Generalized Extreme Value methods
- Transform 40-yard dash times to a speed scale for interpretation
- Evaluate bias, RMSE, and convergence behavior through simulation
- Assess how estimator stability changes as record length increases

## Methods

The analysis treats annual fastest 40-yard dash times as block extremes. Since smaller times indicate better performances, times are transformed to the negative-time scale so that faster performances correspond to larger values.

Monte Carlo simulations are used to generate annual block minima, fit GEV models, compute return levels, and evaluate finite-sample performance across different record lengths.

## Tools Used

- R
- R Markdown
- `dplyr`
- `ggplot2`
- `extRemes`
- Monte Carlo simulation
- Extreme Value Theory

## Key Outputs

- GEV model fitting for annual extreme performances
- Return-level estimation on negative-time and speed scales
- Bias and RMSE summaries
- Convergence diagnostics across record lengths
- Knitted HTML report with figures and results

## Repository Structure

```text
analysis/
    nfl_wr_gev_simulation.Rmd

results/
    nfl_wr_gev_simulation.html

appendix/
    Simulation-Based Verification.pdf