# Basel III Credit Risk RWA & Capital Requirements Project

## Overview

This project calculates credit risk Risk-Weighted Assets (RWA) and capital requirements for a mortgage loan portfolio in preparation for the Basel III framework implementation on 1 January 2024. The analysis covers both the standardized and Internal Ratings-Based (IRB) approaches using loan data.

## Objective

* Calculate credit risk RWA under both the standardized and IRB approaches.
* Compare the results from these two approaches.
* Use logistic regression to model Probability of Default (PD) for the portfolio.
* Handle missing collateral values by applying a default Loan-to-Value (LTV) ratio of 0.45.
* Create effective visualizations to communicate the analysis results.

## Dataset Description

The dataset used is `Mortgage_default` with the following key columns:

* **BAD:** Loan status indicator (1 = defaulted/seriously delinquent, 0 = paid).
* **MORTDUE:** Amount due on an existing mortgage.
* **VALUE:** Value of current property.
* **JOB:** Occupational categories.
* **YOJ:** Years at present job.
* **DEROG:** Number of major derogatory reports.
* **DELINQ:** Number of delinquent credit lines.
* **CLAGE:** Age of oldest credit line in months.
* **NINQ:** Number of recent credit inquiries.
* **CLNO:** Number of credit lines.
* **DEBTINC:** Debt-to-income ratio.

## Methodology

* Data cleaning and handling missing collateral values with default LTV = 0.45 where applicable.
* Logistic regression to estimate Probability of Default (PD) for mortgage loans.
* Calculation of Risk-Weighted Assets (RWA) using Basel III standardized and IRB formulas.
* Visualization of key metrics and risk parameters using suitable data visualization tools.
* Comparison and interpretation of RWA results from both approaches.

## Files in this Repository

* `database_completed.xlsx` — Cleaned and completed database including RWA calculations and other derived metrics.
* `pd_regression.ipynb` — Jupyter notebook containing the Probability of Default regression model and related analysis.
* `credit_analysis_report.pdf` — Written report detailing analysis steps, calculations, and findings.
* `credit_analysis_presentation.pdf` — Presentation summarizing the project results and key points.

## How to Use

1. Review the cleaned dataset and RWA calculations in `database_completed.xlsx`.
2. Open and explore the logistic regression modeling process in `pd_regression.ipynb`.
3. Read the detailed analysis and methodology in the `credit_analysis_report.pdf`.
4. Use the presentation file `credit_analysis_presentation.pdf` for a summarized overview of the project.

