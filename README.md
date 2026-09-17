# Riyadh Residential Property Valuation

Code for the MSc dissertation comparing hedonic regression, XGBoost and CatBoost on Saudi Ministry of Justice residential transactions in Riyadh, 2020–2025.

## Contents

- `project.ipynb`: data cleaning, feature engineering, model training, evaluation and SHAP analysis
- `requirements.txt`: Python packages used
- `results/`: output tables reported in the dissertation

## Data

The data are public residential transaction records from the Saudi Ministry of Justice, included in this repository in the same folder as the notebook:

- `transactions_2020_Q1.xlsx` to `transactions_2023_Q4.xlsx` (16 files)
- `transactions_2025_Q1.xlsx` to `transactions_2025_Q4.xlsx` (4 files)
- `indicators_riyadh_2024_Q1.xlsx` to `indicators_riyadh_2024_Q4.xlsx` (4 files, aggregated indicators only, since deal-level records were not published for 2024)

## Results

The `results` folder contains the tables produced by the notebook, including model comparisons, error analysis, hedonic coefficients, cross-validation and SHAP summaries. Running the notebook recreates these files, along with the cleaned dataset and trained models, which are not included because of their size.

## How to run

1. Install Python 3.14
2. Install the packages: `pip install -r requirements.txt`
3. Open `project.ipynb` and run all cells from top to bottom

## Note

XGBoost 3.4.0 or later is required. Earlier versions handle the district variable differently and give lower results.
