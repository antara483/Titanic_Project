# 🛳 Titanic Survival Prediction Preprocessing Project

A data preprocessing project on the Titanic dataset, preparing the data for machine learning models to predict passenger survival. This project focuses on cleaning, encoding, scaling, and handling outliers to make the dataset **ML-ready**.

## 🖼️ Model Output

Here’s how the Boxplots Before Outlier Removal looks:

![Confusion Matrix - Before Outlier Removal](images/Before%20Outlier%20Removal.png)

And here’s the Boxplots After Outlier Removal:

![Accuracy Score - After Outlier Removal](images/After%20Outlier%20Removal.png)

Dataset[https://www.kaggle.com/datasets/yasserh/titanic-dataset]

### Tools: Python, Pandas, NumPy, Matplotlib/Seaborn, Sklearn
---

## 📋 Project Overview

The Titanic dataset contains information about passengers aboard the Titanic, including demographics, ticket information, and survival status. Machine learning models cannot work effectively with raw data, so preprocessing is a crucial step.

This project covers:

1. **Data Exploration**
   - I started by exploring the dataset to understand its structure. I checked the data types of each column, looked for missing values, and identified which features were numerical and which were categorical.

2. **Handling Missing Values**
   - Next, I dealt with the missing data. I filled the missing values in the Age column using the median, and for the Embarked column, I used the mode.
   - I also dropped the Cabin column since it had too many missing values and wasn’t useful for the analysis.

3. **Encoding Categorical Variables**
   - After cleaning, I converted categorical columns like Sex and Embarked into numeric form using one-hot encoding.
   - I made sure to use the drop_first parameter to avoid multicollinearity issues.

4. **Feature Scaling**
   - To prepare the data for modeling, I standardized numerical features such as Age and Fare using StandardScaler.
   - This step ensured all values were on the same scale (mean = 0, standard deviation = 1).

5. **Outlier Detection and Handling**
   - I visualized Age and Fare using boxplots to check for outliers. Then, I used the IQR method to remove extreme outliers and make the dataset more consistent.

6. **ML Readiness**
   - After completing all preprocessing steps, my dataset became clean, encoded, scaled, and free from outliers — fully ready for applying machine learning models like Logistic Regression, Random Forest, or SVM.

---


