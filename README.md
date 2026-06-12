PCA Formative Assignment — Group 62

This project implements Principal Component Analysis (PCA) from scratch using NumPy only, applied to the Africa Economic, Banking and Systemic Crisis dataset. The goal is to reduce an 11-feature matrix to a lower-dimensional space while retaining as much variance as possible.
Dataset

Source: Kaggle — Africa Economic, Banking and Systemic Crisis Data
Shape: 1,059 rows × 14 columns (11 numeric features used)
Non-numeric columns: case, cc3, country, banking_crisis — handled before PCA
Missing values: Imputed with column means using NumPy nanmean
Features used (11): year, systemic_crisis, exch_usd, domestic_debt_in_default, sovereign_external_debt_default, gdp_weighted_default, inflation_annual_cpi, independence, currency_crises, inflation_crises, banking_crisis (encoded)

Repository Structure
PCA-Formative-Group62/
│
├── Template_PCA_Formative_2_Group62.ipynb   # Main notebook (all outputs visible)
├── african_crises.csv                        # Dataset
├── Contribution_Sheet_Group62.pdf            # Task allocation and contribution sheet
└── README.md                                 # This file
Implementation Steps
StepDescription1Load CSV, separate non-numeric columns, encode banking_crisis as 0/12Impute NaNs with column means (np.nanmean)3Standardize: z = (x − μ) / σ4Compute covariance matrix: Xᵀ · X / (n − 1)5Eigendecomposition via np.linalg.eig6Sort eigenvalues descending, compute explained variance ratios7Select components dynamically at 80% cumulative variance → 7 PCs8Project standardized data onto top-7 eigenvectors (1,059 × 11 → 1,059 × 7)9Visualize before PCA (year vs systemic_crisis) and after PCA (PC1 vs PC2)
Results
PCVariance ExplainedCumulative125.34%25.34%213.19%38.53%312.24%50.77%410.48%61.25%59.14%70.39%68.64%79.03%77.28%86.31%
7 components retained → 80% of total variance preserved.
Libraries Used
LibraryPurposenumpyAll numerical computationmatplotlibVisualizations only
No sklearn or any other ML libraries were used.
How to Run

Open Template_PCA_Formative_2_Group62.ipynb in Google Colab
Upload african_crises.csv to /content/
Run all cells top to bottom — all outputs are pre-saved in the notebook

Group Members

Sarah Gasaro
Nina Bwiza Cyndy

Task Contributions
See Contribution_Sheet_Group62.pdf for the full contribution and meeting attendance log.
