# PCA Formative Assignment — Group 62

This project implements Principal Component Analysis (PCA) from scratch using NumPy only, applied to the Africa Economic, Banking and Systemic Crisis dataset. The goal is to reduce an 11-feature matrix to a lower-dimensional space while retaining as much variance as possible.

## Dataset
- **Source:** Kaggle — Africa Economic, Banking and Systemic Crisis Data
- **Shape:** 1,059 rows × 14 columns (11 numeric features used)
- **Non-numeric columns:** case, cc3, country, banking_crisis — handled before PCA
- **Missing values:** Imputed with column means using NumPy nanmean
- **Features used (11):** year, systemic_crisis, exch_usd, domestic_debt_in_default, sovereign_external_debt_default, gdp_weighted_default, inflation_annual_cpi, independence, currency_crises, inflation_crises, banking_crisis (encoded)

## Repository Structure

PCA-Formative-Group62/

├── Template_PCA_Formative_2_Group62.ipynb

├── african_crises.csv

├── Contribution_Sheet_Group62.pdf

└── README.md

## Results
7 components retained → 80% of total variance preserved.

## Libraries Used
- **numpy** — All numerical computation
- **matplotlib** — Visualizations only

No sklearn or any other ML libraries were used.

## How to Run
1. Open [Template_PCA_Formative_2_Group62.ipynb](Template_PCA_Formative_2_Group62.ipynb) in Google Colab
2. Upload [african_crises.csv](african_crises.csv) to `/content/`
3. Run all cells top to bottom

## Group Members
- Sarah Gasaro
- Nina Bwiza Cyndy

## Task Contributions
See [Contribution_Sheet_Group62.pdf](file:///C:/Users/EVOTECH/Downloads/BSE%20Group%20Assignments%20_%20Task%20Sheet_Mathematics%20for%20Machine%20Learning_Formative%202%20-%20Principle%20Component%20Analysis_Cohort%203_Group%2062]%20-%201.pdf) for the full contribution and meeting attendance log.
