# Credit Default Prediction – ML Benchmark

This project is a refresher on basic machine learning models applied to credit risk.  
It benchmarks several models on a small loan dataset to predict the probability of default and compute expected loss.

## Contents
- `notebook/credit_default_prediction.ipynb` – main analysis  
- `data/loan_data.csv` – input data  
- `pyproject.toml` – dependencies for reproducible runs with uv  

## Models Tested
- DummyClassifier (baseline)
- Logistic Regression
- Polynomial Regression (via feature expansion)
- Decision Tree
- KNN
- Random Forest
- Gradient Boosting

Each model is evaluated using:
- ROC AUC  
- Confusion matrix  
- Mean Squared Error  

Then the more adapted will be used to predict:
- Probability of default (PD)  
- Expected loss (EL = PD × LGD × EAD)

## How to Run
Install dependencies with uv:
uv sync
uv run jupyter lab
Open the notebook and run all cells.

## Goal
Provide a compact example of credit risk modeling and ML benchmarking for learning and academic purposes.
