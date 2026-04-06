# 📊 Student Performance Prediction (Machine Learning Project)

## 📌 Overview

This project predicts a student's **exam score** based on academic and lifestyle factors using Machine Learning techniques.

---

## 🎯 Problem Statement

To predict the **Exam Score** of students using features like:

* Study Hours per Day
* Attendance Percentage
* Previous Grade
* Assignments Completed
* Sleep Hours
* Internet Usage Hours

---

## 📁 Dataset

* Synthetic dataset (500 rows)
* Includes:

  * Noise
  * Missing values (~5%)
  * Outliers

---

## 🔍 Exploratory Data Analysis (EDA)

* Checked dataset structure (`shape`, `info`, `describe`)
* Handled missing values using **median imputation**
* Removed duplicates
* Handled outliers using **IQR capping**
* Performed univariate & bivariate analysis

---

## 🤖 Models Used

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* PCA (for dimensionality reduction)
* GridSearchCV (for hyperparameter tuning)

---

## 📈 Results

| Model             | R² Score               |
| ----------------- | ---------------------- |
| Linear Regression | ~0.24                  |
| Decision Tree     | Negative (overfitting) |
| Random Forest     | Improved after tuning  |
| PCA + Models      | Reduced performance    |

---

## 🏆 Final Model

**Random Forest Regressor (without PCA) + GridSearchCV**

---

## 📊 Evaluation Metrics

* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)
* R² Score

---

## 🔮 Prediction Example

Input:

* Study Hours = 6
* Attendance = 85
* Previous Grade = 70
* Assignments = 8
* Sleep = 7
* Internet Usage = 2

👉 Predicted Exam Score ≈ **61**

---

## 🧠 Key Insights

* Study hours and attendance positively affect performance
* High internet usage negatively impacts scores
* Sleep contributes moderately

---

## 🚀 Future Improvements

* Use real-world datasets
* Try advanced models (XGBoost)
* Feature engineering
* Deploy as a web application

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib
