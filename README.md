Adult Income Classification – Predicting Income Brackets from Demographic Data
🧠 Project Overview
This project addresses a well-established supervised learning problem using the UCI Adult Income Dataset. The objective is to build a robust and interpretable model that predicts whether an individual earns more than $50K per year, based on a range of demographic and employment-related attributes.

Designed as a full-cycle machine learning workflow, the project covers every stage — from raw data preprocessing and exploratory analysis to feature engineering, model building, tuning, and performance evaluation. The final deliverable is a high-performing classifier optimized for F1-score, suitable for deployment or integration into a decision-support tool.

📁 Repository Contents
File Name	Description
adults_income.ipynb	Complete Jupyter notebook with code, EDA, preprocessing, modeling, and insights
income_data_cleaned.csv	Cleaned dataset used for training and testing all models

📊 Dataset Summary
Source: UCI Machine Learning Repository

Observations: ~48,000 rows

Features: 14 demographic and work-related variables (both categorical and numerical)

Target Variable: income (Binary – <=50K or >50K)

📌 Feature Examples:
age, education, marital-status, occupation, relationship, race, sex, hours-per-week, native-country, etc.

🔍 Project Pipeline
1. 📖 Exploratory Data Analysis (EDA)
Visualized class distributions and demographic breakdowns

Identified data imbalance and correlations between variables

Detected and examined outliers

2. 🧹 Data Cleaning & Preparation
Removed records with missing or inconsistent values

Standardized and grouped categorical variables

Engineered relevant features for better signal extraction

3. ⚙️ Feature Engineering
Applied Label Encoding and One-Hot Encoding where appropriate

Scaled numerical features to normalize ranges

Transformed skewed variables for model stability

4. 🤖 Model Development
Implemented and compared multiple classification algorithms:

Logistic Regression

Decision Tree

Random Forest

Support Vector Machine (SVM)

XGBoost (Tuned)

Stacked Ensembles & Voting Classifiers

5. 🔍 Model Optimization
GridSearchCV and threshold tuning were used to maximize F1-score

Handled class imbalance using scale_pos_weight and threshold calibration

📈 Model Evaluation
Evaluated model performance using metrics suitable for imbalanced classification:

Accuracy

Precision

Recall

F1-score (Primary Metric)

Confusion Matrix

ROC-AUC

✅ Final Model Performance (Tuned XGBoost):
Precision: 0.6761

Recall: 0.7970

F1 Score: 0.7316

ROC-AUC: 0.9269

This tuned XGBoost model achieved the best balance between precision and recall and was finalized as the production-ready model.

🔬 Key Insights
Education, hours-per-week, and occupation emerged as the most influential features in income prediction.

Ensemble and stacked models provided competitive performance but were slightly outperformed by the tuned XGBoost in terms of F1-score.

Threshold optimization proved critical in boosting F1 performance for imbalanced targets.

🧰 Tools & Technologies
Languages: Python (Jupyter Notebook)

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost

Model Selection: GridSearchCV, StratifiedKFold, VotingClassifier, StackingClassifier

🚀 Future Enhancements
Integrate LightGBM and CatBoost for further boosting comparison

Automate feature selection using recursive methods or SHAP values

Deploy the final model using Streamlit or Flask for real-time predictions

Build a simple front-end UI to allow users to test the model with custom inputs

