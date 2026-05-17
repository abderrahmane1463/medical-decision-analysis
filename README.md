<h1 align="center">Medical Decision Analysis — Diabetes Case Study</h1>

<p align="center">
  <em>Diabetes prediction using logistic regression combined with utility-based decision theory to recommend treatment vs. monitoring</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
</p>

---

## Overview

A medical decision analysis project that applies probabilistic modelling and utility theory to support clinical decision-making under uncertainty. A logistic regression model is trained on the Pima Indians Diabetes Dataset to estimate individual diabetes probability, and a utility-based decision rule then recommends either early treatment or continued monitoring — balancing the cost of missed diagnoses against unnecessary interventions.

## Features

- Logistic regression classifier for diabetes probability estimation
- Expected utility framework: explicit utility matrix for treatment vs. monitoring outcomes
- Decision boundary analysis with probability thresholds tuned to clinical priorities
- ROC curve and AUC evaluation
- Probability distribution and utility comparison visualisations
- Full theoretical exposition in the accompanying PDF report

## Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python |
| Modelling | scikit-learn (Logistic Regression) |
| Data Analysis | pandas, numpy |
| Visualisation | matplotlib |
| Notebook | Jupyter / Google Colab |

## Project Structure

```
medical-decision-analysis/
├── BIO_STAT.ipynb              # Full analysis: modelling, utility calculations, visualisations
├── BIO_STAT.ipynb - Colab.pdf  # PDF export of the notebook
├── BIO_STAT.pdf                # Theoretical report on medical decision analysis
└── diabetes.csv                # Pima Indians Diabetes Dataset (UCI)
```

## Results / Key Insights

- The logistic regression model achieves solid discriminative performance on the Pima dataset, with the ROC curve demonstrating clear separability between diabetic and non-diabetic patients
- Applying a utility-based decision rule rather than a fixed 0.5 probability threshold meaningfully reduces false negatives — which carry higher clinical cost than false positives in a diabetes screening context
- The analysis demonstrates that optimal decision-making under medical uncertainty requires explicitly encoding the asymmetric costs of different error types, not just maximising accuracy

---

<p align="center">Made by <a href="https://github.com/abderrahmane1463">Cherfaoui Houssam Abderrahmane</a></p>
