# 🛳 Titanic Survival Prediction Preprocessing Project

A data preprocessing project on the Titanic dataset, preparing the data for machine learning models to predict passenger survival. This project focuses on cleaning, encoding, scaling, and handling outliers to make the dataset **ML-ready**.

---

## 📋 Project Overview

The Titanic dataset contains information about passengers aboard the Titanic, including demographics, ticket information, and survival status. Machine learning models cannot work effectively with raw data, so preprocessing is a crucial step.

This project covers:

1. **Data Exploration**
   - Checking data types (`dtypes`)
   - Detecting missing values
   - Understanding numerical and categorical features

2. **Handling Missing Values**
   - Filling missing `Age` values using **median**
   - Filling missing `Embarked` values using **mode**
   - Dropping unnecessary columns like `Cabin`

3. **Encoding Categorical Variables**
   - Converted `Sex` and `Embarked` to numeric using **one-hot encoding**
   - Handled the “drop_first” parameter to avoid multicollinearity

4. **Feature Scaling**
   - Standardized numerical features (`Age`, `Fare`) using **StandardScaler**
   - Ensures features are on the **same scale (mean=0, std=1)**

5. **Outlier Detection and Handling**
   - Visualized `Age` and `Fare` using **boxplots**
   - Removed extreme outliers using the **IQR method**

6. **ML Readiness**
   - Dataset is now clean, encoded, scaled, and free from extreme outliers
   - Ready for building ML models like Logistic Regression, Random Forest, or SVM

---


