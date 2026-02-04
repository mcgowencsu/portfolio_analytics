# Data Analytics for Appointment No-Shows

## Overview

This repository contains a Jupyter notebook that analyzes an EHR dataset containing appointment data to understand variables related to appointment no-shows.

The notebook includes data preparation, statistical analysis, and predictive modeling using binary classification models. Multiple modeling approaches are used to better understand relationships between independent variables and appointment no-shows.

---

## Exploratory Analysis

The workflow examines relationships between independent variables and appointment no-shows to identify potential patterns prior to formal modeling.

---

## Data Loading and Cleaning

Data is loaded using SQLAlchemy. Database connection details are stored in an external configuration file that is not included in this repository in order to prevent exposing credentials in a public codebase.

---

## Statistical Significance

Logistic regression is used to assess statistical associations between independent variables and appointment no-shows. This phase emphasizes interpretability and effect size estimation.

* Wald tests are used to evaluate p-values and odds ratios
* Odds ratios (ORs) are reported to quantify changes in the odds of no-shows associated with each variable

---

## Predictive Modeling

Gradient boosting models are used to complement logistic regression by capturing nonlinear effects and interactions.

Both tree-based and linear models are trained to evaluate predictive performance.

Models explored include:

* Logistic regression
* Gradient boosting models (LightGBM, XGBoost, CatBoost)

Model performance is assessed using ROC–AUC and precision–recall metrics. Gradient boosting models demonstrate similar discrimination performance, with LightGBM performing competitively relative to XGBoost and CatBoost.

These models are used both to evaluate predictive performance and to assess relative variable importance across modeling approaches.
