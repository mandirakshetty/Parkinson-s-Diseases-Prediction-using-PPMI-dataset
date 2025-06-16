# Parkinson-s-Diseases-Prediction-using-PPMI-dataset

This project aims to **predict the stage of Parkinson’s Disease** using clinical and neurological assessment data from the **Parkinson’s Progression Markers Initiative (PPMI)**. By leveraging machine learning algorithms and statistical analysis, the project explores how early symptoms and biomarker data can be used to classify disease progression stages effectively.

---

## 📌 Objective

- Analyze the PPMI dataset for missing values and patterns.
- Engineer relevant features such as symptom scores.
- Perform Exploratory Data Analysis (EDA) to understand distributions and correlations.
- Apply and compare classification algorithms: **Random Forest**, **Logistic Regression**, **SVM**, and **XGBoost**.
- Evaluate model performance and determine the most effective classifier.
- Identify the most important features contributing to Parkinson's stage prediction.

---

## 📁 Dataset Description

- **Source:** [Parkinson’s Progression Markers Initiative (PPMI)](https://www.ppmi-info.org/)
- **Format:** CSV (cleaned version)
- **Key Columns:**
  - `np1slpn`, `np1fatg`, `np1pain`, `np1urln`, `np1cnfn` – Symptom assessments
  - `stage` – Target variable representing Parkinson’s Disease stage
  - `patno` – Patient ID (removed during preprocessing)

---

## 📊 Workflow Overview

### 1. 🔍 Data Preprocessing
- Detect and visualize missing values
- Drop unnecessary identifiers
- Apply mean imputation for missing features
- Engineer a new feature: `symptom_score` (sum of key symptoms)

### 2. 📈 Exploratory Data Analysis
- Dataset shape, types, and summary
- Distribution of symptom scores
- Correlation heatmap
- Stage distribution bar plot
- Pairplots of key symptom features

### 3. 🤖 Model Training and Evaluation
- **Train/Test Split** using 80/20 ratio
- Models applied:
  - Random Forest
  - Logistic Regression
  - Support Vector Machine (SVM)
  - XGBoost
- Evaluation Metrics:
  - Accuracy
  - Classification Report
  - Confusion Matrix

### 4. 🌟 Feature Selection and Importance
- Feature importance plot (XGBoost)
- Model retraining on top 10 features

### 5. 📊 Model Comparison
- Bar plot comparing accuracies of all models
---

## 🛠️ Technologies & Libraries

- **Programming Language:** Python
- **Libraries:**
  - `pandas`, `numpy`, `matplotlib`, `seaborn`
  - `scikit-learn` – model building and evaluation
  - `xgboost` – advanced gradient boosting
- **Visualization:** Heatmaps, Histograms, Pairplots, Bar Plots

---

## 🧪 License

This repository is intended **for educational and academic use only**. Please refer to the [PPMI Terms of Use](https://www.ppmi-info.org/access-data-specimens/download-data/) for dataset licensing and compliance.

