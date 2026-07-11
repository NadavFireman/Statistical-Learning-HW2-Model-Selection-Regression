# Statistical Learning - Model Selection & Regularized Regression (HW2)

**Home Assignment 2 (Grade 94, M.Sc. Data Science, HIT). Five problems on model selection and regularization — applied selection methods reconciled against each other, plus hand-derived estimator theory.**

## Overview
Model selection worked end-to-end on three datasets — household income vs. expenditure in Haifa, psychometric scores across three cities, and Titanic survival: information criteria, cross-validation and regularization paths compared and reconciled, closing with closed-form theory for the OLS, Ridge and LASSO estimators.

## Key Features
- **Model Selection Suite:** Best-subset by adjusted R², forward/backward/stepwise by AIC, and Leave-One-Out CV — including sex × income interactions and square-root/log transforms selected empirically.
- **Regularized Regression:** Relaxed LASSO (LASSO selection, then OLS refit) and Elastic Net, tuned with k-fold cross-validation.
- **Logistic Regression:** Titanic survival with a logit link, regularized via Elastic Net (l1_ratio = 0.7).
- **Nonparametric Bootstrap:** 1,000-iteration confidence intervals, with the full bootstrap distribution plotted per coefficient.
- **Estimator Theory (by hand):** Closed-form expectation, variance and consistency of the OLS, Ridge and LASSO estimators.

## Repository Structure
- `Statistical_Learning_HW2.ipynb`: Full solution notebook — all five problems.
- `Statistical_Learning_HW2.pdf`: PDF export of the executed notebook.
- `haifa_res.csv` / `psych_data.txt` / `titanic.csv`: Datasets (Q1–Q3).
- `Assignment_Instructions_2.pdf`: Original course assignment.
