# 📊 Student Performance Prediction (Machine Learning Project)

## 📌 Overview

This project predicts a student's **Exam Score** using Machine Learning techniques based on academic performance, lifestyle habits, and categorical factors.

---

## 🎯 Problem Statement

To predict the **Exam Score** of students using:

### 🔹 Numerical Features

* Study Hours per Day
* Attendance Percentage
* Previous Grade
* Assignments Completed
* Sleep Hours
* Internet Usage Hours

### 🔹 Categorical Features

* Gender
* Parental Education
* Study Method

---

## 📁 Dataset

* Synthetic dataset (500 rows)
* Includes:

  * Noise
  * Missing values (~5%)
  * Outliers
  * Categorical variables

---

## 🔍 Exploratory Data Analysis (EDA)

### ✔ Basic Checks

* `df.shape`, `df.info()`, `df.describe()`
* `df.head()`, `df.tail()`

### ✔ Data Cleaning

* Handled missing values:

  * Numerical → Mean/Median
  * Categorical → Mode
* Removed duplicates
* Handled outliers using **IQR method**

### ✔ Feature Analysis

* Univariate analysis (distribution of features)
* Bivariate analysis (feature vs target relationships)
* Correlation heatmap

---

## 🔄 Data Preprocessing

### ✔ Encoding Categorical Data

* Applied **One-Hot Encoding (`pd.get_dummies`)**
* Converted categorical variables into numerical format

### ✔ Important Note

* Encoding was done **before train-test split**
* Ensured **same feature structure** during prediction using:

```python
new_data = new_data.reindex(columns=X_train.columns, fill_value=0)
```

---

## 🤖 Models Used

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* PCA (for dimensionality reduction)
* GridSearchCV & RandomizedSearchCV (for tuning)

---

## 📈 Results

| Model             | Performance                       |
| ----------------- | --------------------------------- |
| Linear Regression | Best among baseline models        |
| Decision Tree     | Overfitting (poor generalization) |
| Random Forest     | Improved after tuning             |
| PCA + Models      | Reduced performance               |

---

## 🏆 Final Model

**Linear Regression (best performing for this dataset)**
(Random Forest also tested with tuning)

---

## 📊 Evaluation Metrics

* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)
* R² Score

---

## 🔮 Prediction on New Data

Example input:

* Study Hours = 6
* Attendance = 85
* Previous Grade = 70
* Assignments = 8
* Sleep = 7
* Internet Usage = 2

👉 Predicted Exam Score ≈ **61**

---

## 🧠 Key Insights

* Study hours and attendance strongly influence performance
* Higher internet usage negatively impacts scores
* Sleep contributes positively
* Categorical factors (study method, parental education) also affect outcomes

---

## ⚠️ Challenges Faced

* Handling categorical variables
* Feature mismatch during prediction
* Model performance issues due to noise and outliers

---

## ✅ Solutions Applied

* One-hot encoding for categorical data
* Used `reindex()` to fix feature mismatch
* Applied proper preprocessing techniques
* Compared multiple models

---

## 🚀 Future Improvements

* Use real-world dataset
* Try advanced models (XGBoost, Gradient Boosting)
* Feature engineering
* Deploy as web app

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 📌 Author

**Your Name**

---
isha 
