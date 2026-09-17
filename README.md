# Riyadh Residential Property Valuation

Code for the MSc dissertation comparing hedonic regression, XGBoost and CatBoost on Saudi Ministry of Justice residential transactions in Riyadh, 2020–2025.

## Contents

- `project.ipynb`: data cleaning, feature engineering, model training, evaluation and SHAP analysis
- `requirements.txt`: Python packages used

## Data

The data are not included in this repository. Download the residential transaction files from the Saudi Ministry of Justice and place them in the same folder as the notebook:

- `transactions_*.xlsx` (2020–2023 and 2025)
- `indicators_riyadh_2024_Q1.xlsx` to `indicators_riyadh_2024_Q4.xlsx`

## How to run

1. Install Python 3.14
2. Install the packages: `pip install -r requirements.txt`
3. Open `project.ipynb` and run all cells from top to bottom

## Note

XGBoost 3.4.0 or later is required. Earlier versions handle the district variable differently and give lower results.
