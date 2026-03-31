# Code_Alpha

A collection of Jupyter Notebook tasks completed for the **Code Alpha** program. This repository currently contains two notebooks focused on applied machine learning workflows and evaluation.

## Repository Contents

- **Codealpha_Task_1.ipynb**
  - End-to-end supervised learning pipeline for a *credit risk / default prediction* problem.
  - Loads training and test CSVs (`cs-training.csv`, `cs-test.csv`).
  - Preprocessing:
    - Drops `Unnamed: 0` index column (if present).
    - Median imputation for missing values (`SimpleImputer`).
    - Feature scaling (`StandardScaler`).
    - Train/validation split with stratification (`train_test_split`).
  - Models trained and evaluated:
    - Logistic Regression
    - Decision Tree
    - Random Forest
  - Evaluation outputs include accuracy, precision, recall, F1, ROC-AUC, classification report, and a confusion matrix heatmap.
  - Additional analysis: Random Forest feature importance plot (top features printed).
  - Final step trains on the full dataset and saves predictions to `credit_risk_predictions.csv`.

- **Code_Alpha_Task_4.ipynb**
  - Large notebook (in size) included in the repo.
  - *Note:* it appears to be a substantial task file; see the notebook itself for full details and outputs.

## Requirements

These notebooks are written for Python (Jupyter) and commonly use:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Install (example):

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run
  Colab 
  task 1 link: https://colab.research.google.com/drive/18m0gkRzhgEWKWAgJ3QAVR0cdPH0Haj1l?usp=sharing
  task 4 link: https://colab.research.google.com/drive/1GSzDTi2dFxcJ6pJs1ekYU-FTWFA7A-7s?usp=sharing
1. Clone the repository.
2. (Task 1) Ensure the dataset files referenced by the notebook are available in the same folder as the notebook:
   - `cs-training.csv`
   - `cs-test.csv`
3. Open the notebooks in Jupyter Notebook / JupyterLab / Google Colab and run the cells in order.

## Notes

- The repository currently contains notebooks only (no packaged Python modules).
- If you rename files or move datasets, update the paths in the notebooks accordingly.