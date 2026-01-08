# student-performance-ml
# 🎓 Student Performance Prediction using Machine Learning

This project builds an end-to-end **Machine Learning system** to predict:
- 📊 **Total student score** (Regression)
- 🏷 **Student grade (A, B, C, D, F)** (Classification)

The project uses a **large-scale dataset (1,000,000 records)** and demonstrates real-world ML practices such as baseline modeling, advanced models, class imbalance handling, and model evaluation.

---

## 📂 Dataset
- Source: Kaggle – Student Performance Dataset
- Size: **1,000,000 rows**
- Features:
  - `weekly_self_study_hours`
  - `attendance_percentage`
  - `class_participation`
- Targets:
  - `total_score` (Regression)
  - `grade` (Classification)

---

## 🧠 Problem Statements

### 1️⃣ Regression
Predict a student's **total score** based on study habits and engagement.

### 2️⃣ Classification
Predict a student's **grade** (A/B/C/D/F).

---

## 🛠️ Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## 🔍 Exploratory Data Analysis
- No missing values
- Realistic feature distributions
- Strong correlation between study hours and total score

---

## 🤖 Models Used

### 🔹 Regression Models
| Model | R² Score |
|-----|---------|
| Linear Regression | ~0.66 |
| Random Forest Regressor | ~0.72 |

### 🔹 Classification Models
| Model | Accuracy |
|-----|----------|
| Logistic Regression | ~70% |
| Random Forest Classifier | ~64% |

> Random Forest improved recall for minority classes (D/F), making it suitable for failure detection.

---

## 📊 Model Evaluation
- MAE, RMSE, R² for regression
- Accuracy, Precision, Recall, F1-score for classification
- Confusion matrix for error analysis

---

## 📈 Key Insights
- Weekly self-study hours are the **dominant predictor** of performance
- Tree-based models handle class imbalance better
- Accuracy alone is not sufficient for fair evaluation

---

## 🚀 How to Predict

```python
score, grade = predict_student(18, 88, 6)
print(score, grade)
