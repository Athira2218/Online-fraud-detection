# Online Fraud Detection Project

This machine learning project focuses on detecting fraudulent online financial transactions using a large, real-world dataset. Fraud detection is a key use-case in fintech, requiring careful handling of imbalanced data and precision-focused models.

---

## Project Overview

- Goal: Identify potentially fraudulent transactions
- Dataset: Over 6 million transactions from GeeksforGeeks
- Techniques Used: Exploratory Data Analysis, SMOTE for class imbalance, Random Forest classifier
- Tools: Python, Pandas, Scikit-learn, Seaborn, Matplotlib

---

## Notebook

You can view and run the full project notebook directly in Google Colab:

[Open in Colab](https://colab.research.google.com/drive/1wPAFc_mD0Z00e232wS_KY4DZsfS6PLxG?usp=sharing)

---

## Dataset Summary

| Feature             | Description                             |
|---------------------|-----------------------------------------|
| type                | Transaction type (TRANSFER, CASH_OUT)   |
| amount              | Transaction amount                      |
| oldbalanceOrg       | Sender's balance before transaction     |
| newbalanceOrig      | Sender's balance after transaction      |
| oldbalanceDest      | Receiver's balance before transaction   |
| newbalanceDest      | Receiver's balance after transaction    |
| isFraud             | Target variable (1 = Fraud, 0 = Legit)  |

---

## Key Steps

- Performed exploratory data analysis to understand transaction patterns and fraud distribution
- Applied SMOTE to address severe class imbalance
- Trained and evaluated a Random Forest classifier
- Evaluated model using precision, recall, F1-score, and ROC-AUC

---

## Model Performance (Fraud vs Non-Fraud)

| Metric       | Fraud (1)  | Non-Fraud (0) |
|--------------|------------|---------------|
| Precision    | 0.68       | 1             |
| Recall       | 0.95       | 1             |
| F1-Score     | 0.79       | 1             |
| Support      | 1620       | 1270904       |

*These metrics were calculated using the classification report from Scikit-learn's `classification_report`.*

Additionally, the **ROC-AUC** score for the model was **0.975**.

---

## How to Use

To run or explore this project in Google Colab:

1. Open the notebook using the link above.
2. If prompted, install additional packages:
   ```python
   !pip install imbalanced-learn


**What I Learned** :


* How to handle real-world class imbalance in fraud datasets

* Use of SMOTE for oversampling the minority class

* Training and tuning Random Forest models for fraud detection

* Evaluating models using precision, recall, F1-score, and ROC-AUC



Author
Name: Athira


Acknowledgements

Dataset sourced from GeeksforGeeks

Libraries used: pandas, numpy, matplotlib, seaborn, scikit-learn, imbalanced-learn
