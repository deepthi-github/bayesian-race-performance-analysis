# Bayesian Race Performance Analysis

## Overview

This project applies Bayesian statistical modelling to analyse cross-country race performance using North East Harrier League race data.

The analysis investigates how race time is influenced by athlete characteristics, course difficulty, pack classification, age group, weather conditions, distance, and elevation.

## Features

- Data cleaning and preprocessing
- Exploratory data analysis
- Correlation heatmap
- Race time distribution analysis
- Bayesian non-conjugate model
- Bayesian normal linear regression
- Interaction model
- Hierarchical Bayesian model
- MCMC diagnostics using trace plots, Gelman-Rubin statistics, and effective sample sizes
- Posterior distribution interpretation

## Technologies Used

- R
- R Markdown
- ggplot2
- dplyr
- JAGS / Bayesian modelling tools
- MCMC diagnostics

## Models Implemented

### Model 1: Non-Conjugate Bayesian Model
Includes athlete-level and course-level random effects to capture individual performance variation and course difficulty.

### Model 2: Bayesian Normal Linear Regression
Models race time using predictors such as course, age, pack, temperature, windspeed, and distance.

### Model 3: Interaction Model
Explores interaction effects such as course-temperature, pack-age, and pack-windspeed.

### Model 4: Hierarchical Bayesian Model
Captures structured variation across courses, packs, age groups, and athlete-level effects.

## Key Findings

- Pack classification has a strong relationship with race time.
- Age shows a moderate positive association with finish time.
- Course difficulty affects performance, with some courses showing higher race time variability.
- Hierarchical Bayesian modelling effectively captures group-level variation across packs, age groups, and courses.
- Environmental variables such as temperature and windspeed have smaller but meaningful effects.

## Files

- `bayesian_race_analysis.Rmd`
- `Bayesian-Methodology.pdf`

## Future Improvements

- Add posterior predictive checks
- Compare models using WAIC or LOO-CV
- Improve convergence for interaction model parameters
- Add interactive visualisations
- Extend analysis with longitudinal athlete-level trends
