# LendingClub Loan Default Prediction

This project analyzes and predicts loan default risk using LendingClub loan data, focusing exclusively on pre-origination borrower and loan characteristics. Five machine learning models are evaluated and compared, with an emphasis on realistic deployment.t

## Data
This project uses the LendingClub loan dataset (2007–2018) on Kaggle: https://www.kaggle.com/datasets/adarshsng/lending-club-loan-data-csv/data

Due to size constraints, raw and cleaned datasets are not included in this repository. They are available via Google Drive:

https://drive.google.com/drive/folders/1u9XB8cEP8Y7i-IPIvZmB0IPqlNs-WQjX

The cleaned dataset can be reproduced by running `01_data_cleaning.ipynb`.

## Methods
- Chronological train / val / test split to prevent temporal leakage  
- Evaluation using the F₂-score to emphasize recall in default prediction  
- Models evaluated: Logistic Regression, Decision Tree, Random Forest, k-Nearest Neighbors, and XGBoost  
- Hyperparameter tuning via time-series cross-validation  
- Interpretability via SHAP values, permutation feature importance, and XGBoost split gain

## Environment
- Python 3.13.5 

