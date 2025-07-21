# 📊 Customer Churn Prediction

This project uses machine learning to **predict customer churn**—identifying which customers are likely to leave a subscription or service based on their historical behavior.

## 🚀 Goal
To build a predictive model that helps businesses proactively retain customers by anticipating churn using available usage, support, and activity data.

---

## 🧠 Models Used
- **Logistic Regression**
- **Decision Tree Classifier**
- **Neural Network (Keras)**
  
All models are evaluated using classification metrics (Precision, Recall, F1-score, AUC).

---

## 🛠 Features
- Uses the [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- Feature engineering on categorical and numerical columns
- Class imbalance handled using **SMOTE**
- Scikit-learn and TensorFlow-based pipelines
- Clear comparison of traditional vs deep learning models

---

## 🧾 Dataset Overview

- `customerID`: Unique identifier
- `tenure`: Number of months the customer has stayed
- `Contract`, `PaymentMethod`, etc.: Categorical features
- `MonthlyCharges`, `TotalCharges`: Numeric spending info
- `Churn`: Target variable (Yes = left, No = stayed)

---

## 🧪 Preprocessing Steps

1. Drop `customerID`
2. Convert `TotalCharges` to numeric
3. Encode categorical features using `LabelEncoder` or `get_dummies`
4. Handle missing values
5. Balance classes using **SMOTE**
6. Scale numeric features using `StandardScaler`

---

## 🔍 Results

| Model              | Accuracy | AUC     |
|-------------------|----------|---------|
| Logistic Regression | ✅ Good baseline, interpretable |
| Decision Tree       | 🟡 Fast, but prone to overfitting |
| Neural Network      | 🚀 Best performance after tuning |

---

## 🧰 Libraries Used

- `pandas`, `numpy`
- `scikit-learn`
- `imbalanced-learn` (for SMOTE)
- `tensorflow` / `keras`
- `matplotlib` / `seaborn` (optional for visualization)
