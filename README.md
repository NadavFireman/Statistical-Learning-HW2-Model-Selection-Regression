# Statistical Learning - Model Selection & Regularized Regression (HW2)

**Home Assignment 2 (Grade 94, M.Sc. Data Science, HIT). Six problems on model selection and regularization — best-subset and stepwise selection, Relaxed LASSO and Elastic Net, logistic regression on the Titanic dataset, nonparametric bootstrap confidence intervals, and hand-derived OLS/Ridge/LASSO estimator theory.**

## Overview
The assignment spans applied model selection and its underlying theory across three datasets — household income vs. expenditure in Haifa, psychometric-exam scores across three cities, and Titanic survival. The core question throughout is how to choose among competing models: comparing information criteria, cross-validation, and regularization paths, and reconciling the models they select. It closes with theoretical derivations — the bias, variance and consistency of the OLS, Ridge and LASSO estimators, and a proof relating AIC to Mallows' Cp under Gaussian errors — plus a probability problem underlying the Wilcoxon rank-sum test.

## Key Features
- **Model Selection Suite:** Best-subset selection by adjusted R², forward/backward/stepwise selection by AIC, and Leave-One-Out CV — applied across datasets and cross-checked where they agree and disagree.
- **Regularized Regression:** Relaxed LASSO (two-stage: LASSO selection then OLS refit) and Elastic Net, each with k-fold cross-validation to tune the penalty, and interpretation of the selected sparse models.
- **Interaction & Non-Linear Terms:** Sex × income interaction tested for a difference in slope; concave income effects captured with square-root and log transformations, selected empirically.
- **Logistic Regression:** Binary survival modeled on the Titanic dataset with a logit link, regularized via Elastic Net (α = 0.7), with odds-ratio interpretation of the coefficients.
- **Nonparametric Bootstrap:** 1,000-iteration bootstrap confidence intervals for model coefficients, with the full bootstrap distributions plotted per coefficient.
- **Estimator Theory (by hand):** Closed-form derivations of the OLS, Ridge and LASSO estimators — expectation, variance and consistency — and a proof that AIC equals Mallows' Cp (up to constants) for Gaussian linear models.
- **Rank-Statistic Probability:** Expectation of the rank sums under the null, the theoretical foundation of the Wilcoxon / Mann-Whitney test.

## Tech Stack
- **Language:** Python
- **Statistics & ML:** statsmodels, scikit-learn, SciPy
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn

## Repository Structure
- `Statistical_Learning_HW2.ipynb`: Full solution notebook — all six problems, with derivations, code and analysis.
- `Statistical_Learning_HW2.pdf`: PDF export of the executed notebook.
- `haifa_res.csv`: Household income and monthly expenditure data (Question 1).
- `psych_data.txt`: Psychometric-exam scores across three cities (Question 2).
- `titanic.csv`: Titanic passenger survival dataset (Question 3).
- `Assignment_Instructions_2.pdf`: Original course assignment.
