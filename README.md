PySpark ML: Housing Regression & Loan Classification
====================================================

Two compact **PySpark** notebooks that turn CSVs into evaluated ML models with reproducible pipelines.

Contents
--------

*   housing-price-prediction.ipynb – KC housing → numeric features → **LinearRegression** → prints **MAE/RMSE/R²**.
    
*   loan-prediction-classification.ipynb – Loan data → median imputation + OHE → **DecisionTree** → prints **Accuracy/ROC-AUC**.


Data 

```bash
data/kc_house_data.csv
data/loan-prediction-train.csv   
```

QuickStart

```bash
python -m venv .venv && source .venv/bin/activate
pip install pyspark jupyter
jupyter notebook
# open and run both notebooks
```

What’s shown
------------

*   Clean Spark ML **pipelines** (impute/encode/assemble → train → evaluate)
    
*   **Reproducible** train/test splits (seed=42)
    
*   Clear metrics printed in-notebook (business-friendly)
