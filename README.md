# Heart Attack Risk Classification on IFLS-5 Data

This repository contains the official code and implementation for the research paper:
**"Machine Learning Approaches for Cardiovascular Disease Classification on Indonesian Population Survey Data"**

## 📌 Overview
This study evaluates seven machine learning algorithms (Logistic Regression, KNN, Decision Tree, Random Forest, Support Vector Machine, Neural Network, and Flexible Discriminant Analysis) to classify doctor-diagnosed heart attack history using the Fifth Wave of the Indonesia Family Life Survey (IFLS-5). 

To handle the extreme class imbalance (~0.98% positive prevalence), the pipeline incorporates:
1. Data preprocessing and standard scaling.
2. Feature selection using **XGBoost Feature Importance** (Selected features: `Diabetes`, `HighCholesterol`, `BMI`, `Weight_kg`).
3. Class imbalance handling via **SMOTE** on training data.

## 📁 Repository Structure
- `IFLS5_HeartAttack_Classification_Pipeline.ipynb` : The primary Jupyter Notebook containing data loading, preprocessing, model training, cross-validation, and holdout evaluation.
- `README.md` : Project documentation and guidelines.

## 🛠️ Requirements & Installation
To run the notebook, install the required packages:
```bash
pip install numpy pandas scikit-learn imbalanced-learn xgboost
