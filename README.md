🛡️ Online Payment Fraud Detection using Machine Learning

📌 Project Overview

This project focuses on building a machine learning model to detect fraudulent online payment transactions. With the rise of digital transactions, fraud detection is crucial for ensuring security and reducing financial risks.

Using Python and popular ML libraries, I analyzed the dataset, performed feature engineering, and trained multiple classification models (Logistic Regression, Random Forest, XGBoost) to identify fraudulent behavior.

📊 Dataset

The dataset contains transactional details such as:

step ⏱️ (time step)

type 💳 (transaction type: CASH_OUT, TRANSFER, etc.)

amount 💰 (transaction amount)

nameOrig, nameDest 👥 (sender and receiver IDs)

oldbalanceOrg, newbalanceOrig, oldbalanceDest, newbalanceDest

isFraud 🚨 (target: 1 = Fraud, 0 = Legit)

🛠️ Tech Stack

Programming Language: Python 🐍

Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn (SMOTE), XGBoost

ML Models: Logistic Regression, Random Forest, XGBoost

📈 Workflow

Data Exploration & Visualization 📊

Distribution of transaction types & amounts

Fraud vs. non-fraud imbalance check

Data Preprocessing 🔄

Encoding categorical variables

Dropping irrelevant columns

Handling class imbalance with SMOTE

Model Training 🤖

Logistic Regression

Random Forest

XGBoost

Evaluation Metrics 📑

Confusion Matrix

Precision, Recall, F1-score

ROC-AUC Curve

📈 Understanding ROC & AUC
🔹 ROC (Receiver Operating Characteristic) Curve

The ROC curve is a plot that shows how well a classification model distinguishes between classes (Fraud 🚨 vs. Non-Fraud ✅).

X-axis: False Positive Rate (FPR) → how many legitimate transactions were incorrectly flagged as fraud.

Y-axis: True Positive Rate (TPR / Recall) → how many frauds were correctly detected.

A good model’s curve hugs the top-left corner of the graph.

🔹 AUC (Area Under the Curve)

The AUC is a single number that summarizes the ROC curve.

AUC = 0.5 → Model is no better than random guessing 🎲

AUC = 1.0 → Perfect classifier 🎯

Closer to 1 → Better fraud detection model

✅ Why It Matters in Fraud Detection

Fraud detection datasets are usually imbalanced (frauds are rare).

Accuracy can be misleading (e.g., predicting "Not Fraud" for all transactions gives 99% accuracy).

ROC-AUC provides a much better measure of whether the model can actually distinguish fraud from legitimate transactions.

In this project, the Random Forest & XGBoost models achieved an AUC of 0.97, meaning they can correctly rank fraud vs. non-fraud transactions 97% of the time.

✅ Results

Achieved ROC-AUC = 0.97

Fraud detection Recall improved to ~83% (catching more fraud cases)

F1-score = 0.85 balancing precision & recall

Reduced false positives by ~15% compared to baseline logistic regression



## 📂 Dataset
The dataset (450MB) is too large to host on GitHub.  
➡️ Download it here: [Google Drive Link](https://drive.google.com/file/d/1WCN9M6B3zDR6gePhrR2omSEPR8LzTJpe/view?usp=drive_link) 
