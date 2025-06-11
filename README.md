# 🚨 Network Intrusion Detection using Machine Learning

This project focuses on building a machine learning-based system to detect network intrusions and classify malicious activities in an IoT environment. It uses a labeled dataset of network flows and applies preprocessing, dimensionality reduction, and classification algorithms to predict threats accurately.

---

## 📂 Dataset

- **Source:** CIC-IoMT 2024 WiFi-MQTT dataset (provided)
- **Files:**
  - `train.csv`: Contains labeled network activity data
  - `test_without_label.csv`: Unlabeled data for final prediction

---

## 📊 Problem Statement

Detect whether a given network traffic record represents **normal** or **malicious** activity. The challenge includes:
- High-dimensional features
- Mixed feature types (categorical and numerical)
- Imbalanced class distribution

---

## 🛠️ Project Workflow

### 1. **Exploratory Data Analysis**
- Null value analysis
- Class distribution check
- Feature types breakdown (object vs numeric)
- Visualizations: Count plots, PCA projections

### 2. **Data Preprocessing**
- Label encoding for categorical features
- Min-Max Scaling for numerical features
- Dimensionality reduction using PCA (to 32 and 16 components)

### 3. **Modeling**
- **Random Forest:** Baseline classifier
- **LightGBM:** Final tuned model
- Grid Search and Hyperparameter Tuning

### 4. **Evaluation**
- Cross-validation F1-score
- Confusion matrix
- ROC-AUC (if applicable)

### 5. **Prediction & Submission**
- Predictions on `test_without_label.csv`
- Final predictions saved as `network_intrusion_predictions.csv`

---

## ✅ Results

| Model       | F1-Score (Validation) |
|-------------|------------------------|
| Random Forest | 0.91                |
| LightGBM (tuned) | **0.98**         |

---

## 📌 Tools & Libraries
Python
Pandas, NumPy, Scikit-learn
LightGBM
Matplotlib, Seaborn
PCA (Dimensionality Reduction)


