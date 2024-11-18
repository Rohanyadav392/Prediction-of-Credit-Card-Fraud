# Prediction-of-Credit-Card-Fraud
We have to build a classification model to predict whether a transaction is fraudulent or not.
## Project Overview
This project tackles the critical issue of detecting fraudulent credit card transactions using machine learning. Fraudulent activities pose financial and reputational risks to financial institutions. Using a real-world anonymized dataset of European credit card transactions, this project implements robust classification models to accurately identify fraud while addressing the challenges of data imbalance, real-time detection, and misclassification costs.
##  Problem Statement
The dataset contains 284,807 transactions, of which only 0.172% are fraudulent, making it highly imbalanced. Fraud detection systems must balance precision (minimizing false positives) and recall (minimizing false negatives) while operating in near real-time to prevent financial losses and ensure customer trust.
## Dataset and Key Features
1. Time: Seconds elapsed since the first transaction.  
2. Amount: Monetary value of the transaction, normalized during preprocessing.  
3. V1–V28: Anonymized features derived from PCA for privacy.  
4. Class: Target variable (`1` for fraud, `0` for non-fraud).  
## Challenges Addressed
- Extreme class imbalance.
- Feature anonymity and lack of direct interpretability.
##  Methodology
1. Data Preprocessing: Addressed missing values, removed outliers, and created cyclic features (`Hour_sin`, `Hour_cos`) for temporal trends.  
2. Class Balancing: Used SMOTE to generate synthetic minority class samples.  
3. Modeling: Built models using Logistic Regression, Decision Tree, and Random Forest, focusing on interpretability and performance.  
4. Evaluation Metrics: Prioritized F1 Score, Precision, Recall, and ROC-AUC due to class imbalance.
## Findings  
- Logistic Regression: Simplicity and precision (F1 Score: 97.98%).  
- Decision Tree: High accuracy and flexibility (F1 Score: 99.89%).  
- Logistic Regression and Decision Tree models were deployed using Streamlit for real-time fraud detection.
## Future Work  
- Incorporate real-time detection using APIs.  
- Explore advanced models like LSTMs for temporal patterns.  
- Enhance interpretability with SHAP or LIME.  
- Implement dynamic model updating to adapt to evolving fraud patterns.  
