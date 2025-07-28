# Credit Card Fraud Detection 🛡️

This project builds a machine learning pipeline to detect fraudulent transactions using a real-world credit card dataset.

---

## 📊 Dataset

The dataset includes anonymized numerical features (`V1` to `V28`), `Amount`, and the target variable `Class`:
- `Class = 0` → Legitimate transaction  
- `Class = 1` → Fraudulent transaction

---

## 🔧 Features & Workflow

### ✔️ Data Loading
- Loaded using `pandas.read_csv()`

### ✔️ Preprocessing
- Standardization of features using `StandardScaler`  
- Feature-target split with `train_test_split`

### ✔️ Modeling
- `RandomForestClassifier` is used for classification

### ✔️ Evaluation
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- ROC Curve and AUC Score

### ✔️ Visualization
- Heatmaps and ROC plots using `matplotlib` and `seaborn`

---
___
# 📘 Method & Function Reference

This document explains every method and function used in the notebook.

---

## 📦 Data Handling & Transformation

| Method         | Description                                              |
|----------------|----------------------------------------------------------|
| `read_csv`     | Loads a CSV file into a pandas DataFrame                 |
| `head`         | Displays the first few rows of the DataFrame             |
| `info`         | Provides metadata including column types and null values |
| `isnull`       | Checks for missing (null) values                         |
| `drop`         | Removes rows or columns from a DataFrame                 |
| `mean`         | Computes the average of values in a Series               |
| `sum`          | Computes the total sum across values                     |
| `value_counts` | Returns count of unique values in a Series               |
| `sort_values`  | Sorts the DataFrame by a specific column                 |
| `tolist`       | Converts a Series or array into a Python list            |

---

## ⚙️ Preprocessing

| Method           | Description                                                     |
|------------------|-----------------------------------------------------------------|
| `StandardScaler` | Standardizes features to zero mean and unit variance            |
| `fit`            | Learns the transformation parameters from the training data     |
| `transform`      | Applies learned transformation to data                          |
| `fit_transform`  | Fits and transforms in one step                                 |

---

## 🎯 Model Training & Evaluation

| Method                | Description                                                        |
|------------------------|--------------------------------------------------------------------|
| `train_test_split`     | Splits data into training and test sets                           |
| `RandomForestClassifier` | Ensemble tree-based classifier from scikit-learn              |
| `fit`                  | Trains the machine learning model                                 |
| `predict`              | Predicts labels for input samples                                |
| `predict_proba`        | Returns the probability estimates of the classes                 |
| `cross_val_score`      | Performs cross-validation scoring of a model                     |

---

## 🧪 Model Evaluation Metrics

| Method                | Description                                                     |
|------------------------|-----------------------------------------------------------------|
| `confusion_matrix`     | Displays TP, TN, FP, FN counts in a matrix form                |
| `classification_report`| Summarizes precision, recall, f1-score                         |
| `roc_curve`            | Computes ROC curve data (TPR vs. FPR)                          |
| `auc`                  | Area Under the Curve (AUC) score from ROC                      |

---

## 📊 Visualization (Matplotlib & Seaborn)

| Method        | Description                                          |
|---------------|------------------------------------------------------|
| `plot`        | Plots basic graphs                                   |
| `figure`      | Initializes a new figure                             |
| `show`        | Renders the plot                                     |
| `tight_layout`| Adjusts layout for readability                       |
| `title`       | Sets the plot title                                  |
| `xlabel`      | Sets the label for the X-axis                        |
| `ylabel`      | Sets the label for the Y-axis                        |
| `xlim`        | Sets the X-axis view limits                          |
| `ylim`        | Sets the Y-axis view limits                          |
| `legend`      | Displays the legend on the plot                      |
| `barplot`     | Seaborn method to plot categorical bar graphs        |
| `heatmap`     | Seaborn method to plot a heatmap (e.g. correlation)  |

---

## 🧱 Pandas Structures

| Term        | Description                            |
|-------------|----------------------------------------|
| `DataFrame` | 2D table-like data structure in pandas |
| `Series`    | 1D array-like object in pandas         |

---



