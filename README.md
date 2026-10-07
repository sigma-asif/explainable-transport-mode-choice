# Explainable Transport Mode Choice

Explainable transport mode choice analysis in Pabna Municipality using ML benchmarking, SHAP, sensitivity analysis, and Qwen3-based evidence-grounded explanations.

## Study Overview

This repository contains the analysis code for an explainable transport mode choice study conducted in Pabna Municipality, Bangladesh.

The study combines machine learning benchmarking, SHAP-based explainability, respondent-level attribution analysis, sensitivity testing, and Qwen3-8B-based evidence-grounded reporting.

The analysis uses survey data from 348 respondents in Pabna Municipality. Seven reported transport modes were consolidated into four functional classes:

- Intermediate
- Public
- Low-cost Personal
- Private/Hired

Six machine-learning classifiers were evaluated under a common stratified out-of-fold framework:

- Random Forest
- XGBoost
- LightGBM
- Gradient Boosting
- SVM-RBF
- Multinomial Logistic Regression

Random Forest achieved the strongest performance in the main model benchmark and was subsequently used for detailed SHAP-based explainability and respondent-level attribution analysis.

## Repository Structure

```text
.
├── 01_model_benchmark_rf_shap.ipynb
├── 02_qwen3_llm_explanations.ipynb
├── 03_sensitivity_excluding_context_variables.ipynb
└── README.md
