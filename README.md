# 📊 IPL Total Runs Prediction Project

This repository contains the Jupyter Notebook `ipl.ipynb`, which analyzes IPL match data and builds predictive models to estimate the **total runs (`total`)** scored in a match.

---

## 📌 Overview

The goal of this project is to explore IPL match data, engineer meaningful features, and compare several machine learning algorithms—including **Gradient Boosting, Random Forest, CatBoost, and Lasso Regression**—to evaluate how well they can predict match totals.

The notebook includes:

* Data cleaning
* Exploratory Data Analysis (EDA)
* Feature engineering
* Model training & comparison
* Evaluation using RMSE, MAE, R², and MAPE

---

## 🗂 Files

* `ipl.ipynb` — Main Jupyter Notebook (analysis, modeling, and visualizations)
* `ipl.csv` — Dataset used inside the notebook (`pd.read_csv("ipl.csv")`)

---

## 🧰 Requirements

Suggested `requirements.txt`:

```
pandas
numpy
scikit-learn
matplotlib
seaborn
catboost
jupyter
```

Install with:

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run the Project

1. Place `ipl.ipynb` and `ipl.csv` in the same directory.
2. Open the notebook via Jupyter:

```bash
jupyter notebook ipl.ipynb
```

3. Run cells in order to load data, perform EDA, build models, and review results.

### Optional: Run as a Python Script

```bash
jupyter nbconvert --to script ipl.ipynb
python ipl.py
```

(You may need to adjust plotting or interactive cells.)

---

## ⚙️ Technical Notes

* Data is loaded using: `df = pd.read_csv("ipl.csv")`.
* Model features include: `venue, bat_team, bowl_team, batsman, bowler, runs, wickets, overs, runs_last_5, wickets_last_5, striker, non-striker`.
* Models used: Gradient Boosting, Random Forest, CatBoost, Lasso.
* Metrics: RMSE, MAE, R², MAPE.
* Pipelines and OneHotEncoding are applied for categorical variables.

---

## ✅ Results

The notebook generates a final comparison table showing the evaluation metrics for each model. See the last notebook cells for detailed outputs.

---

## 💡 Future Improvements

* Add more advanced feature engineering (player stats, form, pitch/venue conditions, etc.)
* Use cross-validation instead of a single train-test split
* Hyperparameter tuning using GridSearchCV or Optuna
* Residual analysis to inspect model errors



