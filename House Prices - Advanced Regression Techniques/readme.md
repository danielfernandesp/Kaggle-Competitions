# 🏠 House Prices - Advanced Regression Techniques

Welcome to my solution for the [Kaggle competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques), where the objective is to predict final sales prices for residential homes based on various features.

---

## 📌 Problem Statement

> Predict the **final sale price** of each home in the test dataset, using 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa.

This competition is a great exercise in:
- Advanced regression modeling
- Feature selection and engineering
- Handling missing data
- Ensemble learning

---

## 📂 Project Structure

```text
📁 House Prices - Advanced Regression Techniques/
📄 README.md          ← Project overview
📊 house_prices.csv   ← Raw dataset (Kaggle provided)
📓 HousePrice_EDA.ipynb      ← Data cleaning and exploratory analysis
📓 Model_Building.ipynb      ← Feature engineering and model training
📓 Final_Model_Submission.ipynb ← Submission-ready pipeline
```

---

## 🔍 Exploratory Data Analysis (EDA)

In the notebook `HousePrice_EDA.ipynb`, I performed:
- Missing value treatment and imputation
- Correlation analysis
- Distribution checks (e.g., log-transforming skewed variables)
- Outlier removal and encoding categorical features

Key insights:
- Neighborhood and overall quality are strong predictors.
- SalePrice distribution is **right-skewed** → log-transform applied.

---

## 🧠 Modeling Techniques

In `Model_Building.ipynb`, I used the following models:

- **Lasso Regression**: For feature selection and regularization.
- **XGBoost Regressor**: For capturing non-linear relationships.
- **Stacking Ensemble**: Combining multiple models to improve performance.

📈 **Final Score (Public Leaderboard):** `0.962`

### 📊 Performance Metrics (Validation Set)
- **Mean Squared Error (MSE):** 277,937,344.00  
- **Mean Absolute Error (MAE):** 8,514.63  
- **R² Score:** 0.9597

These metrics indicate a strong model fit, with low prediction error and high explanatory power.

---

## 🧪 Feature Engineering Highlights

- One-hot encoding of categorical variables
- Creation of new features (e.g., total square footage)
- Log transformation of skewed numerical variables
- Robust scaling to standardize the inputs

---

## 🛠️ Tools and Libraries

- Python 3
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`, `xgboost`, `lightgbm`
- `scipy`, `statsmodels`

---

## 💡 Lessons Learned

- Handling missing data differently per feature type is essential.
- Regularization techniques help prevent overfitting on small datasets.
- Stacking improves predictive performance, especially when models are diverse.

---

## 🛄 Submission

The final predictions were generated from the stacking ensemble and submitted to Kaggle. The submission file was prepared in `submission_1_random_forest.csv`.

---

## 📌 References

- [Competition Page](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
- [Stacking Techniques - scikit-learn Docs](https://scikit-learn.org/stable/modules/ensemble.html#stacking)

---

## 📬 Let’s connect

If you have any feedback or ideas for improvements, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/danielfernandesp) or check out more projects on [GitHub](https://github.com/danielfernandesp).
