# Applied Statistics Project

A collection of three applied statistics analyses covering Bayesian inference, Bayesian regression, hierarchical modeling, and survival analysis using Python.

The project demonstrates both classical and Bayesian statistical approaches across different real-world datasets.

## Project Structure

This repository contains three Jupyter notebooks:

1. `Bayesian_Linear_Regression_Penguins.ipynb`
2. `Survival_Analysis_Rossi.ipynb`
3. `Bayesian_Analysis_Breast_Cancer.ipynb`

---

## 1. Bayesian Linear Regression – Palmer Penguins

This notebook analyzes the relationship between **penguin flipper length and body mass** using both classical and Bayesian regression.

### Methods

- Exploratory data analysis
- Classical Ordinary Least Squares (OLS) regression
- Bayesian linear regression using PyMC
- Prior and posterior distributions
- MCMC sampling and convergence diagnostics
- Credible intervals
- Posterior predictive sampling
- Comparison between classical and Bayesian estimates
- Hierarchical Bayesian regression by penguin species

The classical OLS and simple Bayesian models produced very similar estimates for the relationship between flipper length and body mass.

The analysis was then extended to a hierarchical model, allowing regression parameters to vary between penguin species.

---

## 2. Survival Analysis – Rossi Recidivism Dataset

This notebook applies survival analysis techniques to the **Rossi recidivism dataset**, where the event of interest is rearrest and many observations are right-censored.

### Methods

- Survival and censoring concepts
- Empirical survival analysis
- Exponential survival model
- Weibull survival model
- Kaplan–Meier estimator
- Nelson–Aalen cumulative hazard estimator
- Survival comparison between groups
- Log-rank test
- Cox proportional hazards regression
- Proportional hazards diagnostics

A key part of the analysis demonstrates why censored observations should not simply be removed and how the Kaplan–Meier estimator incorporates their information.

The Cox model was also used to examine how individual characteristics are associated with the hazard of rearrest.

---

## 3. Bayesian Analysis – Breast Cancer Wisconsin Dataset

This notebook explores Bayesian statistical inference using the **Breast Cancer Wisconsin dataset**.

The analysis focuses on estimating and comparing probabilities of malignant tumors while demonstrating several fundamental Bayesian concepts.

### Methods

- Beta-Bernoulli modeling
- Analytical Bayesian posterior calculation
- Bayesian inference with PyMC and MCMC
- Sequential Bayesian updating
- Comparison of credible and classical confidence intervals
- Bootstrap confidence intervals
- Posterior predictive sampling
- Bayesian and classical hypothesis testing
- Bayes Factors
- Savage-Dickey density ratio
- Analysis across tumor radius groups
- Hierarchical Bayesian modeling
- Shrinkage
- Model comparison using WAIC

The analytical and MCMC posterior estimates were highly consistent.

The analysis also demonstrates how sequential Bayesian updating produces the same final posterior as analyzing all observations simultaneously.

Independent and hierarchical Bayesian models were later compared across tumor-radius groups.

---

## Statistical Concepts Demonstrated

Across the three notebooks, the project covers:

- Classical vs. Bayesian inference
- Regression modeling
- Prior and posterior distributions
- MCMC sampling
- Convergence diagnostics
- Credible and confidence intervals
- Posterior predictive distributions
- Hierarchical models
- Partial pooling and shrinkage
- Bayesian hypothesis testing
- Bayes Factors
- Model comparison
- Survival functions
- Right censoring
- Hazard functions
- Cox proportional hazards models

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- SciPy
- PyMC
- ArviZ
- Statsmodels
- Lifelines
- Google Colab

## Files

`Bayesian_Linear_Regression_Penguins.ipynb` – classical and Bayesian linear regression with hierarchical modeling.

`Survival_Analysis_Rossi.ipynb` – survival analysis, censoring, Kaplan–Meier estimation, and Cox regression.

`Bayesian_Analysis_Breast_Cancer.ipynb` – Bayesian inference, sequential updating, hierarchical models, and Bayesian model comparison.
