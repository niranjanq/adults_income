Adult Income Classification – Predicting Income Brackets Using Census Data
📌 Project Overview
This project tackles a classic supervised machine learning problem using the UCI Adult Income dataset. The goal is to build a predictive model that determines whether an individual earns more than $50K per year based on various demographic and employment-related attributes.

It includes comprehensive steps from data preprocessing and exploration to model building, evaluation, and insights. The entire pipeline is implemented in Python using standard machine learning libraries.

📁 Repository Contents
File Name	Description
adults_income.ipynb	Jupyter notebook with EDA, preprocessing, model training, evaluation, and insights
income_data_cleaned.csv	Cleaned dataset used for training and testing the ML models

📊 Dataset Description
The dataset originates from the UCI Machine Learning Repository and includes approximately 48,000 records with 14 features (both categorical and numerical).

🎯 Target Variable
income: Binary classification – whether income is <=50K or >50K

🧾 Features
age, education, workclass, marital-status, occupation, relationship, race, sex, hours-per-week, native-country, etc.

🔍 Project Workflow
1. 📖 Exploratory Data Analysis (EDA)
Analyzed distribution of income with respect to key features

Visualized class imbalance

Studied correlations and outliers

2. 🧹 Data Cleaning
Removed missing or inconsistent entries

Consolidated categorical values

Handled class imbalance

3. ⚙️ Feature Engineering
Label encoding and one-hot encoding

Feature scaling for numerical columns

Transformation of skewed features

4. 🤖 Model Building
Trained and evaluated the following models:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Support Vector Machine (SVM)

5. 📈 Model Evaluation
Used appropriate metrics for imbalanced classification:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

6. 🧠 Insights
Identified most influential features on income (e.g., education level, hours worked, occupation)

Compared model performances and selected the best trade-off model

🧰 Technologies Used
Python (Jupyter Notebook)

pandas, NumPy

matplotlib, seaborn

scikit-learn

📌 Key Learnings
Handling real-world datasets with missing and noisy data

Feature transformation and encoding

Comparison of multiple classification algorithms

Proper model validation and interpretation

📬 Future Enhancements
Hyperparameter tuning using GridSearchCV or RandomizedSearchCV

Implement cross-validation for more robust evaluation

Try boosting algorithms (XGBoost, LightGBM)

Deploy the final model using Flask or Streamlit

