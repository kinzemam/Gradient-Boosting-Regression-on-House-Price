# 🏠 California Housing Price Prediction using Gradient Boosting

## 📌 Overview
This project uses Gradient Boosting Regression to predict median house prices based on demographic and geographic features from the California Housing dataset. The objective is to build an accurate regression model through proper preprocessing, minimal exploratory data analysis, and hyperparameter tuning.

---

## 📂 Dataset
- California Housing Dataset (1990 Census)
- Target variable: `median_house_value`
- Features include housing, population, income, and location-related attributes
- Contains one categorical feature: `ocean_proximity`

---

## 🔍 Exploratory Data Analysis
Minimal exploratory data analysis was performed to:
- Inspect dataset structure and feature types
- Identify and handle missing values
- Check feature ranges and target distribution

---

## 🧹 Data Preprocessing
- Missing values in `total_bedrooms` were imputed using the median
- The categorical feature `ocean_proximity` was encoded using one-hot encoding
- Irrelevant identifier columns were removed
- Data was split into training and testing sets

---

## 🤖 Model
**Gradient Boosting Regressor**

Gradient Boosting is an ensemble learning technique that builds models sequentially, where each model learns from the residuals of previous models to improve predictions.

---

## ⚙️ Model Configuration
The final model was trained with:
- `n_estimators = 300`
- `learning_rate = 0.05`
- `max_depth = 5`

These hyperparameters were selected after experimentation to balance bias and variance.

---

## 📊 Evaluation Metrics
The following regression metrics were used:
- R² Score
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

---

## ✅ Results
- R² Score ≈ 0.80 
- Mean Absolute Error ≈ $34,000  
- Root Mean Squared Error ≈ $50,000  

The model explains a significant portion of variance in housing prices while maintaining reasonable prediction accuracy.

---

## 🧠 Key Observations
- Lower learning rate with more estimators improved performance
- Moderate tree depth captured important feature interactions
- Gradient Boosting effectively handled non-linear relationships

---

## 🏁 Conclusion
The Gradient Boosting Regressor demonstrated strong performance on the California Housing dataset. With appropriate preprocessing and tuning, the model proved effective for structured regression tasks and serves as a solid baseline for future enhancements.

---

## 🚀 Future Work
- Implement XGBoost or LightGBM for improved performance
- Perform feature engineering to extract additional insights
- Apply cross-validation for more robust evaluation

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
