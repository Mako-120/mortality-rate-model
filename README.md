# Mortality Rate in Poland — Lee-Carter Model (1989–2023)

Stochastic mortality modelling for Poland using the Lee-Carter framework, with ARIMA and Gradient Boosting forecasts of the mortality index κ. Includes analysis of COVID-19 excess mortality impact on long-term projections.

---

## Overview

This project models the evolution of mortality rates in Poland across 8 age groups and 35 years (1989–2023), then forecasts mortality for 2024–2033.

The analysis is structured in three stages:

1. **Descriptive analysis** — age-specific mortality rates on a log scale, visualising improvements over the post-communist transformation period.
2. **Lee-Carter decomposition** — extracting the mortality index κ and age-specific sensitivity coefficients β via Singular Value Decomposition (SVD).
3. **Forecasting κ** — comparing ARIMA(0,1,0) with Gradient Boosting Regressor, evaluated on a held-out test set with multiple train/test splits.

---

## Data Sources

| File | Description | Source |
|---|---|---|
| `POLdeath.txt` | Deaths by single year of age and calendar year | [Human Mortality Database (HMD)](https://www.mortality.org/) |
| `population_pl.csv` | Mid-year population by age group | [GUS — Statistics Poland](https://stat.gov.pl/) |

---
