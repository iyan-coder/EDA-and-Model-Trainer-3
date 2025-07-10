# 📊 ML Project Workspace – Churn, Loan, Banking Market & Flight Prediction

This repository contains structured work on real-world ML problems including **Customer Churn**, **Loan Prediction**, **Banking Market Response**, and **Flight Price Prediction**. It focuses on robust data pipelines, exploratory data analysis (EDA), preprocessing, model evaluation using multiple metrics with **recall** emphasized for imbalanced scenarios.

> 🛠 This workspace is designed to evolve. New datasets will follow a reusable pipeline and evaluation logic for consistency and clarity.

---

## ✅ Current Datasets

### 1. 📉 Customer Churn Prediction

* **Goal**: Identify customers likely to churn.
* **Key Steps**:
  - Cleaned and mapped binary features
  - OneHotEncoded categorical variables
  - Scaled features with `StandardScaler`
  - Balanced data using `SMOTE`
  - Trained:
    - Logistic Regression
    - Random Forest
    - AdaBoost
    - Gradient Boosting
    - XGBoost
  - Evaluated with:
    - Accuracy
    - Precision, Recall
    - F1 Score
    - ROC AUC
  - **Focus**: Maximize **recall** to catch at-risk customers

---

### 2. 💰 Loan Prediction

* **Goal**: Predict loan approval status.
* **Key Steps**:
  - EDA on categorical and numeric features
  - Handled missing values, label/one-hot encoding
  - Compared classifiers with emphasis on **recall**
* **Best Model**: Logistic Regression (good balance of interpretability and performance)

---

### 3. 🏦 Banking Market Response (Term Deposit Subscription)

* **Goal**: Predict if a customer will subscribe to a term deposit.
* **Key Steps**:
  - Cleaned and encoded socio-economic features
  - Explored job, education, and campaign-related behaviors
  - Balanced the dataset using SMOTE
  - Focused on avoiding **false negatives** (missed interested clients)
  - Compared models using recall, F1-score, ROC AUC

---

### 4. ✈️ Flight Price Prediction (Deep Learning)

* **Goal**: Predict flight ticket prices based on travel information using **Deep Learning**.
* **Key Steps**:
  - Extracted features from date/time columns
  - Converted text data (e.g. airlines, source, destination) using encoding
  - Scaled continuous variables
  - Trained regression models including:
    - Linear Regression
    - Random Forest Regressor
    - XGBoost Regressor
    - ✅ **Neural Network (Deep Learning)** using Keras/TensorFlow
  - **Metrics Used**:
    - MAE, MSE, RMSE, R² Score
  - **Emphasis**: Low **RMSE** and strong **generalization** using DL model

---

## 🔍 Evaluation Highlights

| Problem | Priority Metric | Why It Matters |
|--------|------------------|----------------|
| Churn | Recall | Catch all at-risk customers |
| Loan | Recall | Avoid missing eligible applicants |
| Bank | Recall | Don’t miss likely subscribers |
| Flight | RMSE / R² | Accurate price estimation using **deep learning** |

---

## 🧪 How to Run

```bash
# Activate your environment
conda activate mlenv  # or virtualenv

# Run Jupyter
jupyter notebook
```
### 🧭 Project Structure
📁 project_root/
│
├── 📄 README.md <- This file
│
├── 📁 TeleCustomerChurnNotebook/ <- VSCode folder with scripts, models, and EDA
│
├── 📁 LoanPredictionProblem/ <- VSCode folder with scripts, models, and EDA
│
├── 📄 BankMarketing.ipynb <- Google Colab notebook (single file)
│
├── 📄 Flight_Prediction.ipynb <- Google Colab notebook (DL-based)
│
└── 📄 requirements.txt <- Project dependencies


### 🚀 What's Next
 * Add datasets in health, fraud detection, and education

 * Modularize reusable preprocessing and training pipelines

 * Convert selected notebooks into end-to-end ML/DL apps

 * Version experiments and models using MLflow

 * Add Docker & cloud deployment support (AWS, Azure, GCP)

### 🙌 Acknowledgments
This project is part of my ML Engineering journey — building toward deployable, production-ready solutions using best practices in data science and MLOps.

> 🔄 Feedback, suggestions, or collaborations are always welcome!


