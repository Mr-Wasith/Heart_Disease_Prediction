# Heart Disease Prediction - Machine Learning Project

This project uses **Machine Learning algorithms** to predict the likelihood of **heart disease** in patients based on various medical attributes such as age, cholesterol levels, blood pressure, and more. It primarily implements **Logistic Regression** and **Random Forest Classifier** for prediction and accuracy comparison.

---

## 📊 Dataset
- **Source:** UCI Heart Disease Dataset
- **File Used:** `heart.csv`
- **Features Include:**
    - Age
    - Sex
    - Chest Pain Type
    - Resting Blood Pressure
    - Serum Cholesterol
    - Fasting Blood Sugar
    - Resting ECG Results
    - Max Heart Rate Achieved
    - Exercise-Induced Angina
    - ST Depression (Oldpeak)
    - Slope of Peak Exercise ST Segment
    - Number of Major Vessels (Ca)
    - Thalassemia Type
- **Target Variable:**
    - `target` (1 = Heart Disease, 0 = Healthy)

---

## 🛠️ Libraries Used
- **numpy** - Numerical operations
- **pandas** - Data loading and processing
- **matplotlib** - Data visualization
- **seaborn** - Heatmaps and distributions
- **scikit-learn** - Machine Learning models, accuracy, train-test split

---

## 📊 Exploratory Data Analysis
- Checked first and last rows for data verification.
- Inspected dataset size, structure, and missing values.
- Generated a **correlation heatmap** to study feature relationships.
- Verified **target class distribution** (healthy vs diseased).

---

## ⚙️ Machine Learning Models Used
### 1️⃣ Logistic Regression
- Simple and interpretable model.
- Trained on **80% of the data**, evaluated on **20% test set**.
- Accuracy measured for both training and test data.

### 2️⃣ Random Forest Classifier
- Ensemble learning model using decision trees.
- Trained using **100 estimators** for robustness.
- Final predictions made using this model.

---

## 🔬 Accuracy Comparison (Example)
| Model                        | Training Accuracy | Test Accuracy |
|-------------------|-------------------|----------------|
| Logistic Regression        | ~85% | ~82% |
| Random Forest Classifier   | N/A (Only test accuracy calculated) | ~90% |

> Actual results might vary based on random seed or train-test split.

---

## 🩺 Predictive System
- Accepts **new patient data** as a tuple (age, sex, cp, trestbps, chol, etc.)
- Reshapes the input to fit the trained model.
- Uses the **Random Forest Classifier** to predict:
    - **0 = Healthy Heart**
    - **1 = Heart Disease Present**

### Sample Prediction
```text
The Person does not have a Heart Disease
or
The Person has a Heart Disease

---
