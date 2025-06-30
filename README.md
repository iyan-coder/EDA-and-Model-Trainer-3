# 📊 ML Project Workspace - Churn & Loan Prediction

This repository contains structured work on **Customer Churn** and **Loan Prediction** problems. It focuses on Exploratory Data Analysis (EDA), feature engineering, preprocessing pipelines, and model evaluation using multiple metrics beyond just accuracy — especially **recall** for imbalanced data scenarios.

> 🛠 This workspace is designed to evolve. As more datasets will be analyzed, their pipelines and evaluation logic will follow the same structure.

---

## ✅ Current Datasets

### 1. 📉 Customer Churn Prediction

* **Goal**: Identify customers likely to churn.
* **Steps done**:

  * Cleaned and mapped binary features
  * Handled multi-category variables via OneHotEncoding
  * Scaled all features with `StandardScaler`
  * Resampled with `SMOTE` to balance class distribution
  * Trained multiple models:

    * Logistic Regression
    * Random Forest
    * AdaBoost
    * Gradient Boosting
    * XGBoost
  * Evaluated using:

    * Accuracy
    * F1 Score
    * Precision, Recall
    * ROC AUC
  * Focused on **recall** to reduce false negatives

### 2. 💰 Loan Prediction

* **Goal**: Predict loan approval.
* **Steps done**:

  * EDA on categorical and numeric features
  * Handled missing values, encoded categories
  * Compared several classifiers
  * Used recall as key metric for approval sensitivity

---

## 🔍 Evaluation Highlights

* **Why Recall Matters**:

  * For churn: catching customers before they leave
  * For loans: avoiding missed approvals for truly eligible applicants

* **Best Models So Far**:

  * Churn: AdaBoost (better recall & ROC AUC)
  * Loan: Logistic Regression (balanced metrics, interpretable)

---

## 🧪 How to Run

```bash
# Activate your environment
conda activate mlenv  # or your virtualenv name

# Run Jupyter or your IDE
jupyter notebook
```

Each dataset has its own `.ipynb` file.

---

## 🧭 Project Structure

```
📁 project_root/
│
├── 📄 README.md           <- This file
├── 📁 notebooks/          <- Notebooks for each dataset
│   
├── 📁 data/               <- Raw and processed CSV files
├── 📁 models/             <- Saved models (if any)
└── 📁 reports/            <- Plots and evaluation reports
```

---

## 🚀 What's Next

* [ ] Add 2-3 more datasets: health, fraud, education, etc.
* [ ] Create reusable pipeline modules
* [ ] Convert selected projects into **end-to-end deployments**
* [ ] Version model experiments with MLflow

---

## 🙌 Acknowledgments

This project is part of my ML Engineering journey — preparing for real-world deployments and research.

> If you're reviewing this repo, feedback is welcome!
