# Data Analytics for Appointment No-Shows

## Overview

This repository contains a Jupyter notebook that analyzes an EHR dataset containing appointment data to understand variables related to appointment no-shows.

The notebook includes data preparation, statistical analysis, and predictive modeling using binary classification models. Multiple modeling approaches are used to better understand relationships between independent variables and appointment no-shows.

---

## Exploratory Analysis

The workflow examines relationships between independent variables and appointment no-shows to identify potential patterns.

---

## Data Loading and Cleaning

Data is loaded using SQLAlchemy. Database connection details are stored in an external configuration file that is not included in this repository in order to prevent exposing credentials in a public codebase.

---

## Feature Evaluation

Both Gradient boosting and logisitic regression models are used to assess importance of factors contributing to no-shows.

Models explored include:
* Gradient boosting models (LightGBM, XGBoost, CatBoost)
* Logistic regression, including Wald Test.

Model performance is assessed using ROC–AUC and precision–recall metrics. 

