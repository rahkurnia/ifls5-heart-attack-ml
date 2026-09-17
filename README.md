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
- `IFLS5_HeartAttack_Classification_Pipeline.ipynb` : The primary Jupyter Notebook containing data loading, preprocessing, feature merging, model training, cross-validation, and holdout evaluation.
- `README.md` : Project documentation and guidelines.

## 📊 Dataset & Data Source
The raw data originates from the **Fifth Wave of the Indonesia Family Life Survey (IFLS-5)** conducted by the RAND Corporation. 
- The dataset used in the code was created by merging relevant IFLS-5 survey modules (e.g., adult health history, anthropometric measurements, and demographic characteristics).
- Raw IFLS-5 data files can be officially requested and downloaded from the RAND Corporation repository: https://www.rand.org/well-being/social-and-behavioral-policy/data/FLS/IFLS.html

## 🛠️ Requirements & Installation
To run the notebook, install the required packages:
pip install numpy pandas scikit-learn imbalanced-learn xgboost

## 🚀 How to Run
1. Clone or download this repository:
   git clone https://github.com/rahkurnia/ifls5-heart-attack-ml.git

2. Navigate to the project directory:
   cd ifls5-heart-attack-ml

3. Open `IFLS5_HeartAttack_Classification_Pipeline.ipynb` using Google Colab or Jupyter Notebook/Lab.

4. Place your merged CSV dataset file (or run the data merging cells within the notebook using the raw IFLS-5 files) into the root working directory.

5. Execute all cells sequentially from top to bottom.
