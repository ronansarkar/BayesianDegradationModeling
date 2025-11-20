# BayesianDegradationModeling

## Description

This project implements a probabilistic Bayesian model to forecast the degradation (integrity over time) of mechanical components. The model's long-term predictions are benchmarked against a traditional Linear Regression model trained on short-term features.

---

## Features

- Implement a Bayesian hierarchical model with MCMC sampling (via NumPyro) to fit an exponential decay curve to component integrity data. The model accounts for both component-specific random effects (`u`, `v`) and the influence of static features (`X1-X5`) via a linear combination (`w`).
- Produce full predictive distributions, including credible intervals for the underlying degradation function and the noisy observations.
- Compare the long-term Bayesian forecast against a Linear Regression model trained on early-life component data (first 10 days) to predict integrity at a specific future point (day 30).
  
---

## Installation

### Recommended Python version

- Python 3.12.2 or above

1. **Install required libraries**
   pip install -r requirements.txt

---


## Usage

1. Run the Jupyter Notebook

## Author

Ronan Sarkar – MSc Data Science, University of Bath
