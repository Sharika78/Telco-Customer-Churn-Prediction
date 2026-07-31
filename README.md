# 📊 Telco Customer Churn Prediction

A Machine Learning project focused on analyzing customer demographics, account details, and subscription services to predict whether a customer will churn (leave the service) or stay.

---

## 📌 Project Overview
Customer churn is a critical metric for telecom companies. Predicting potential churners allows businesses to take proactive retention measures. In this project, a **Logistic Regression** model was trained and evaluated on the Telco Customer Churn dataset.

* **Target Variable:** `Churn` (1 = Yes, 0 = No)
* **Dataset Size:** 7,043 rows, 21 initial columns

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Kaggle Notebooks

---

## 🔄 Workflow & Steps

1. **Data Ingestion:** Loaded the dataset directly from Kaggle.
2. **Data Preprocessing & Cleaning:**
   * Converted `TotalCharges` to numeric and handled missing values using median imputation.
   * Dropped uninformative features like `customerID`.
   * Mapped the target variable `Churn` to binary values (1 and 0).
3. **Feature Encoding & Splitting:**
   * Applied **One-Hot Encoding** (`pd.get_dummies`) for categorical variables.
   * Split data into **Training (80%)** and **Testing (20%)** sets.
4. **Feature Scaling:** Scaled numeric features using `StandardScaler` to ensure optimal convergence.
5. **Model Training & Evaluation:**
   * Trained a **Logistic Regression** model.
   * Evaluated model metrics using Accuracy, Classification Report, and Confusion Matrix.

---

## 📈 Model Performance & Results

* **Accuracy:** `80.70%`

### Classification Report Summary:
* **Precision (No Churn / Class 0):** 0.85
* **Recall (No Churn / Class 0):** 0.89
* **F1-Score (Churn / Class 1):** 0.61

---

## 💡 Key Takeaways
* **Feature Scaling matters:** Applying `StandardScaler` prevented model convergence warnings and slightly improved test accuracy from `80.34%` to `80.70%`.
* **Contract and Monthly Charges** play a significant role in customer retention patterns.
*
