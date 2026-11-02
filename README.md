# Healthcare Project

## Overview

This project applies machine learning techniques to a healthcare dataset to analyse and predict patient test results. The project includes data preprocessing, exploratory data analysis, feature engineering, handling class imbalance using SMOTE, model training, evaluation and explainability analysis.

## Dataset and Target Variable

The project uses a healthcare dataset containing patient-related and medical information.

The original **Test Results** variable contains three categories:

- Normal
- Abnormal
- Inconclusive

For this project, the target was converted into a binary classification problem:

- **Normal:** 0
- **Abnormal and Inconclusive:** 1

## Feature Engineering

Two additional features were created:

- **Length of Stay** – calculated using the admission and discharge dates.
- **Billing per Day** – calculated using the billing amount and length of stay.

Outliers in numerical features were identified using the IQR method and capped where necessary.

## Exploratory Data Analysis

The project includes:

- Target variable distribution analysis
- Histograms for numerical features
- Outlier analysis
- Correlation heatmap

## Machine Learning Models

The following models were trained and evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- Naive Bayes
- Gradient Boosting
- K-Nearest Neighbours (KNN)
- Support Vector Machine (SVM)

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score

## Handling Class Imbalance

SMOTE (Synthetic Minority Over-sampling Technique) was applied to the training data. Model performance was compared before and after applying SMOTE.

## Model Evaluation and Explainability

The project also includes:

- Hyperparameter tuning using GridSearchCV
- ROC curve comparison
- Confusion matrix analysis
- Classification report
- Performance comparison across gender groups
- SHAP analysis for model explainability
- Feature importance analysis

## Project Findings

The `Findings` folder contains visualisations generated during the project, including:

- `confusion_matrix.png` – Confusion Matrix
- `heatmap.png` – Correlation Heatmap
- `histograms.png` – Distribution of Numerical Features
- `outlier.png` – Outlier Analysis
- `roc.png` – ROC Curve Comparison
- `shap.png` – SHAP Analysis
- `smote_comparison.png` – Model Performance Before and After SMOTE
- `target.png` – Target Variable Distribution

## Project Structure

```text
Healthcare_Project/
│
├── Findings/
│   ├── cm.png
│   ├── heatmap.png
│   ├── histograms.png
│   ├── outlier.png
│   ├── roc.png
│   ├── shap.png
│   ├── smote_comparison.png
│   └── target.png
│
├── Healthcare.ipynb
├── healthcare_dataset.csv
└── README.md
```

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- SHAP

## How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries.
3. Ensure `healthcare_dataset.csv` is in the same directory as `Healthcare.ipynb`.
4. Open the notebook using Jupyter Notebook or JupyterLab.
5. Run the cells sequentially to reproduce the analysis and results.

## Author

**Manikeshwari Matta**

MSc Computing in Human Centred AI
