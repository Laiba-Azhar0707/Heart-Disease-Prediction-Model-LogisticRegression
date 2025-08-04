# 🩺 Heart Disease Prediction Using Logistic Regression

This project uses a **Logistic Regression** model to predict the likelihood of heart disease in patients based on clinical attributes. It combines five public cardiovascular datasets into one of the largest heart disease datasets available for research.

---

## 📊 Dataset Overview

The dataset contains **918 records** with **11 key medical features**:

- `Age`: Patient’s age
- `Sex`: Male/Female
- `ChestPainType`: Type of chest pain (e.g., ASY, ATA, NAP, TA)
- `RestingBP`: Resting blood pressure
- `Cholesterol`: Serum cholesterol level
- `FastingBS`: Fasting blood sugar > 120 mg/dl (1 = true)
- `RestingECG`: Electrocardiogram results
- `MaxHR`: Maximum heart rate achieved
- `ExerciseAngina`: Angina induced by exercise (Y/N)
- `Oldpeak`: ST depression induced by exercise
- `ST_Slope`: Slope of the ST segment (Up, Flat, Down)
- `HeartDisease`: **Target** (1 = heart disease, 0 = normal)

---

## 🧠 Objective

To build a **Logistic Regression model** that:
- Predicts heart disease presence based on medical attributes
- Helps understand which features impact the risk
- Supports early detection of cardiovascular risk

---

## 🔧 Technologies Used

- Python 🐍
- Pandas & NumPy
- Scikit-learn (LogisticRegression, train_test_split, metrics)
- Matplotlib / Seaborn (for visualization)

---

## 📌 Project Steps

1. **Data Cleaning & Preprocessing**
   - Removed nulls & converted all categorical columns using One-Hot Encoding
2. **Model Building**
   - Trained Logistic Regression with `max_iter=1000`
3. **Evaluation**
   - Used accuracy, precision, recall, F1-score, ROC-AUC
4. **Feature Analysis**
   - Identified top features contributing to heart disease risk

---

## 📈 Results

- ✅ Achieved solid classification accuracy : 0.8532608695652174

Classification Report:
               precision    recall  f1-score   support

           0       0.80      0.87      0.83        77
           1       0.90      0.84      0.87       107

    accuracy                           0.85       184
   macro avg       0.85      0.86      0.85       184
weighted avg       0.86      0.85      0.85       184


Confusion Matrix:
 [[67 10]
 [17 90]]

Roc_AUC score:
 0.8556256827284863


- 🔍 Identified key predictors like Chest Pain Type, ST Slope, and Exercise-Induced Angina



